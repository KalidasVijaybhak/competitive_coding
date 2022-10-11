# Bubble Sort

https://www.youtube.com/watch?v=nmhjrI-aW5o


## Observation 

>  for each iteration the freatest value will be placed at the end

      #include <iostream>

      using namespace std;
      void bubbleSort(int size,int array[]);
      int main()
      {
       int size;
       int i ,j;
       int array[100];

       cout<<"Enter the size of array: ";
       cin>>size;

       cout<<"Enter the elements: ";
       for(int i = 0;i<size;i++){
           cin>>array[i];
       }

       cout<<endl;
        for(int i = 0;i<size;i++){
           cout<<array[i]<<endl;
       }
       cout<<endl;
        bubbleSort(size,array);
 
    for(int i = 0;i<size;i++){
     cout<<array[i]<<endl;
     }

    }

    void bubbleSort(int size,int array[]){
        int i,j;
    
    int temp;
    for(i = 0;i<size-1;i++){
        for(j = 0;j<size-i-1;j++){
            if(array[j]>array[j+1]){
            temp = array[j];
            array[j] = array[j+1];
            array[j+1] = temp;}
        }
    }
    }
