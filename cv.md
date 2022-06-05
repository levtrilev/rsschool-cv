# Lev Trishankov
**React JS Software Engeneer**

![Lev Trishankov](/assets/images/myphoto.jpg "Lev Trishankov, React JS Software Engeneer")

### Contact information:
```
 Address:  21-4 Bolshaya Filiovskaya Street, Moscow
 Phone: +7 964 783 3461, Email: levtrishankov@gmail.com, levtrishankov@gmail.com
 Discord: Lev Trishankov (@levtrilev)
 Telegram: @Lev_Trishankov
 Github: @levtrilev
```
### OBJECTIVE 	
***Develop React JS applications as B2B  products***

### SUMMARY
<p>I have a good experience as a Project manager, Product manager, IT department manager, but since my young ages most of all I like to create software with my own hands, so I decided not to deny myself this pleasure</p>

### WORK EXPERIENCE

02/2022 – 06/2022
**React JS Software Engeneer, DBA, SureCRM project, (pet project)**
- Composed React JS/Recoil application for interfacing with REST API
- Composed a Postgre SQL database & PostgREST REST-API app as a backend for the project

06/2021 – 11/2021
**Flatter/Dart Software Engeneer, Planner project, (pet project)**
- Composed Flatter/Dart application for interfacing with REST API
- Composed MS SQL database & .NET Core REST-API app as a backend for the project

07/2020 – 04/2021
**C# .Net/Alef Software Engeneer, ALPHAMEDEX — SUPPLIER OF MEDICAL DEVICES, Saint Petersburg, remotely**
- Composed C# .Net(WinForms)/Alef application in the part of CRM, sales, inventory, settlements and financial accounting

09/2019 – 08/2020
**student of School 21 (Moscow branch of School 42)**
- C language programming, Algorithms, Data structures, Basic Linux library. Carried out educational projects level 1 - level 6

07/2017 – 07/2020
**Project Manager, Rosatom, Moscow**
- Led the project of development and implementation of the NPP main equipment repair management system (EAM-system)

### SKILLS
**React-JS Typescript Recoil Material-UI REST-API SQL PostgreSQL** 

_Flutter/Durt async_redux Dart C# C Python Microsoft-SQL-Server
Product-owner Project-manager_

### ENGLISH
- Upper Intermediate (B2) test Rosatom Academy 2018
- TOEFL 570 points 1992 New York – official certificate

### EDUCATION
- 1988 Moscow Power Engineering Institute
- 2000 ACCA / Enterprise Finance Management. Financial University under the Government of the RF
- 2018 Rosatom Academy. Business English, Upper Intermediate graduate test

### MY CODE EXAMPLES
[My SUREcrm github repo](https://github.com/levtrilev/surecrm)

#### My Codewars example:
```
Challenge(4kyu): Complete the function to return true when its argument is an array that has 
the same nesting structures and same corresponding length of nested arrays as the first array. 
For your convenience, there is already a function 'isArray(o)' declared and defined that 
returns true if its argument is an array, false otherwise.
 // should return true
[ 1, 1, 1 ].sameStructureAs( [ 2, 2, 2 ] );          
[ 1, [ 1, 1 ] ].sameStructureAs( [ 2, [ 2, 2 ] ] );  

 // should return false 
[ 1, [ 1, 1 ] ].sameStructureAs( [ [ 2, 2 ], 2 ] );  
[ 1, [ 1, 1 ] ].sameStructureAs( [ [ 2 ], 2 ] ); 

My Solution:

Array.prototype.sameStructureAs = function (other) {

const checkArr = function (arr1, arr2) {
  let isSame = true;
  let isArr1 = isArray(arr1);
  let lenArr1 = isArr1 ? arr1.length : 0;
  let isArr2 = isArray(arr2);
  let lenArr2 = isArr2 ? arr2.length : 0;
  if ((isArr1 !== isArr2) || ((isArr1 && isArr2) ? lenArr1 !== lenArr2 : false) ) {
      return false;
  }
  for (let i = 0; i < arr1.length; i++) {
    isArr1 = isArray(arr1[i]);
    lenArr1 = isArr1 ? arr1[i].length : 0;
    isArr2 = isArray(arr2[i]);
    lenArr2 = isArr2 ? arr2[i].length : 0;
    isSame =
      isArr1 === isArr2 && lenArr1 === lenArr2 &&
      (isArr1 && isArr2 ? checkArr(arr1[i], arr2[i]) : true);
    if (!isSame) return false;
  }
  return isSame;
};
    return checkArr(this, other);
};
```