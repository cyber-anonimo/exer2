# exer2
#include<iostream>
#include<cstdlib>
#include<ctime>
#define vetor 50
#define sorte 120
using namespace std;

int main(){

	int numero[vetor];
	int conta;
	srand(time(NULL));

	for(int i = 0; i < vetor; i++){
		numero[i] = rand() % sorte;
	}

	for(int i = 0; i < vetor; i++){
		int posterior = 1;		
		if(i > 0){
			posterior = numero[i - 1];
		}
		cout << " posicao: " << i << "numero sorteado: " << numero[i] << " resultado: " << numero[i] * posterior << "\n";
	}

system("pause");
return 0;
}
