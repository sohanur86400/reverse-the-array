# reverse-the-array
//This code give perfect result but more space complexity.
 #include<iostream>
using namespace std;

void reverse(int array[],int size){
    int i;
    int arr[size];
    for(i=0;i<size;i++){
    				arr[i]=array[i];
				}
    for(i=0;i<size;i++){
    array[i]=arr[size-1-i];
}
}
void print(int array[],int size){
    int i;
    cout << "Reversed array are:";
    for(i=0;i<size;i++){
        cout << array[i]<<endl;;
    }
}
int main(){
    int n,i;
    cout << "Enter arrays element number."<< endl;
    cin >> n;
    int array[n];
    cout << "Enter elemnt one by one"<<endl;
    for(i=0;i<n;i++){
        cin >> array[i];
    }
    reverse(array,n);
    print(array,n);
    return 0;
}
