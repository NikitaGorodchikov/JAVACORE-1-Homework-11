# JAVACORE-1-Homework-11

## Задача "Понимание JVM"
### ClassLoaders
1. JVM находит классы, которые используются в данном коде (JvmComprehension, Object, Integer);
2. Они подгружаются в ClassLoader'ы (только если классы были найдены, в противном случае: ClassNotFoundException): Application ClassLoader, Platform ClassLoader, Bootstrap ClassLoader;
3. Далее происходит связывание (Linking), то есть подготовка классов к выполнению (Verify, Prepare, Resolve);
4. Далее выполняются static инициализаторы и инициализаторы static полей (`main()`, `printAll()`);
### Области памяти
5. ![Распределение памяти](https://raw.githubusercontent.com/NikitaGorodchikov/JAVACORE-1-Homework-11/master/%D0%94%D0%BE%D0%BF%D0%BE%D0%BB%D0%BD%D0%B5%D0%BD%D0%B8%D0%B51.bmp);
6. Программа выполняется;
7. Производиться сборка мусора;
