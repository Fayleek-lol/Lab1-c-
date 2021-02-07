#include <iostream>

using namespace std;

int main()
{
    int size;
    cout << "Введите размерность массива: ";
    cin >> size;
    
    int A[size];
    int B[size];
    
    for (int i = 0; i < size; i ++){
        cout << "A [" << i << "] = ";
        cin >> A[i];
        cout << "B [" << i << "] = ";
        cin >> B[i];
    }
    
    int size3 = size + size; 
	int arr[size3];
	
    for (int i = 0; i < size3; i++){
        if (i < size){
            arr[i] = A[i];} 
        else {
	        arr[i] = B[i - size];
        }
   }
   
    for(int i = 1; i < size3; ++i)
	{
		for(int k = 0; k < size3 - i; k ++)
		{
			if(arr[k] < arr[k + 1])
			{
				int temp = arr[k];
				arr[k] = arr[k + 1];
				arr[k + 1] = temp;
			}
		}
	}
	
	for(int i = 0 ; i < size3 ; i++){
		if((i == 0) || (arr[i] < arr[i-1]) && (i == (size3 - 1) || (arr[i]) > arr[i+1]))
			cout << arr[i] << " ";
    }
	    
    return 0;
}
