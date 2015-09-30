# Problema_8
#include <iostream> 

using namespace std; 


    void ordenar_numeros(int *p, int n){ 
        int Temp; 
         for(int i=0;i<n;i++)
                for(int j=0;j<n-1;j++) 
                	if(*(p+j)<*(p+j+1)){
                    
                        Temp=*(p+j); 
                        *(p+j)=*(p+j+1); 
                        *(p+j+1)=Temp;} 
                        } 
	void mostrar_numeros(int *p, int n){
		for(int i=0;i<n;i++) 
                    cout<<*(p+i)<<endl; 
	}
	

        main(){ 

        int ntotal,n; 
        cout<<"Ingrese cantidad de numeros : "; 
        cin>>ntotal; 
        int array[ntotal],*puntero; 
        puntero=array;
        for(int i=0;i<ntotal;i++){ 
            cout<<"Ingrese numero "<<i+1<<": "; 
            cin>>n; 
            array[i]=n; 
            } 
            cout<<endl<<"Numeros ordenados de menor a mayor: "<<endl; 
            ordenar_numeros(puntero,ntotal); 
            mostrar_numeros(puntero,ntotal);
            
            
    	return 0;
            
        } 
