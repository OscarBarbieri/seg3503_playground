# Lab 02 - Equivalence Classes / Classes d'équivalence

## Exercice 1 - Manual Test Cases / Cas de test manuels

### Registration App Test Results

| TC | Résultats Escomptés | Résultats Actuels | Verdict |
|---|---|---|---|
| TC01 | Enregistrement accepté | Congratulations John Doe! You are now a member of our site. ![TC01 Input](assets/Test1_E.png) ![TC01 Result](assets/Test1_R.png) | Succès |
| TC02 | Échec / UserName obligatoire | Size must be between 6 and 12 + Wrong UserName format ![TC02 Input](assets/Test2_E.png) ![TC02 Result](assets/Test2_R.png) | Succès |
| TC03 | Échec / FirstName obligatoire | Congratulations Doe! You are now a member of our site. ![TC03 Input](assets/Test3_E.png) ![TC03 Result](assets/Test3_R.png) | Échec |
| TC04 | Échec / LastName obligatoire | Congratulations John! You are now a member of our site. ![TC04 Input](assets/Test4_E.png) ![TC04 Result](assets/Test4_R.png) | Échec |
| TC05 | Échec / FirstName invalide | Wrong FirstName format ![TC05 Input](assets/Test5_E.png) ![TC05 Result](assets/Test5_R.png) | Succès |
| TC06 | Échec / LastName invalide | Wrong LastName format ![TC06 Input](assets/Test6_E.png) ![TC06 Result](assets/Test6_R.png) | Succès |
| TC07 | Échec / Email sans @ | Wrong Email format ![TC07 Input](assets/Test7_E.png) ![TC07 Result](assets/Test7_R.png) | Succès |
| TC08 | Échec / Email sans domaine | Wrong Email format ![TC08 Input](assets/Test8_E.png) ![TC08 Result](assets/Test8_R.png) | Succès |
| TC09 | Échec / Email obligatoire | Wrong Email format ![TC09 Input](assets/Test9_E.png) ![TC09 Result](assets/Test9_R.png) | Succès |
| TC10 | Échec / Age invalide (< 18) | must be >= 18 ![TC10 Input](assets/Test10_E.png) ![TC10 Result](assets/Test10_R.png) | Succès |
| TC11 | Échec / Age négatif | must be >= 18 ![TC11 Input](assets/Test11_E.png) ![TC11 Result](assets/Test11_R.png) | Succès |
| TC12 | Échec / Age non-numérique | Server error / NumberFormatException ![TC12 Input](assets/Test12_E.png) ![TC12 Result](assets/Test12_R.png) | Non-concluant |
| TC13 | Échec / City obligatoire | City is a dropdown — Halifax selected, registration accepted ![TC13 Input](assets/Test13_E.png) ![TC13 Result](assets/Test13_R.png) | Non-concluant |
| TC14 | Échec / Code postal invalide | Wrong Postal Code format ![TC14 Input](assets/Test14_E.png) ![TC14 Result](assets/Test14_R.png) | Succès |
| TC15 | Échec / Code postal obligatoire | Wrong Postal Code format ![TC15 Input](assets/Test15_E.png) ![TC15 Result](assets/Test15_R.png) | Succès |

---

### JUnit Parameterized Runner Results

![JUnit Results](assets/junit_results.png)

---

## Exercice 2 - Tests JUnit

### Exécution des tests avec bin/test

![Résultats bin/test](assets/bin_test_results.png)

### Cas de test explicites (DateTest.java)

![Résultats DateTest](assets/DateTest.png)

### Cas de test paramétrisés - Succès (DateNextDateOkTest.java)

![Résultats DateNextDateOkTest](assets/DateNextDateOkTest.png)

### Cas de test paramétrisés - Exceptions (DateNextDateExceptionTest.java)

![Résultats DateNextDateExceptionTest](assets/DateNextDateExceptionTest.png)