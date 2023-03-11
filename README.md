# CompilerConnect-API

<img alt="Javascript" src="https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E"/> <img alt="Nodejs" src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white"/>

API to run C++ code on the cloud :)

BASE URL: //

### Required request body

```
{
    "inputCheck": "true", //true || false
    "language": "cpp", //cpp
    "input": "8 9 5 2 13",
    "code": "#include <iostream>
             using namespace std;

             void bubbleSort(int arr[], int n)
             {
                 int i, j;
                 for (i = 0; i < n - 1; i++)
                     for (j = 0; j < n - i - 1; j++)
                         if (arr[j] > arr[j + 1])
                             swap(arr[j], arr[j + 1]);
             }

             void printArray(int arr[], int size)
             {
                 int i;
                 for (i = 0; i < size; i++)
                     cout << arr[i] << " ";
                 cout << endl;
             }

             int main()
             {
                 int arr[5];
                 for (int i = 0; i < 5; i++)
                 {
                     cin >> arr[i];
                 }

                 bubbleSort(arr, 5);
                 printArray(arr, 5);
                 return 0;
             }",
    
}
```

### Endpoints

- `/execCode`

**Response:**

```
{
    output: '2 5 8 9 13'
}
```
