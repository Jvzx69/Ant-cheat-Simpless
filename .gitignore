#include <iostream>
#include <windows.h>
#include <cstdlib>
#include <stdio.h>
#include <vector>

using namespace std;

int main(){
    vector<char*> appsIlicitos={"Cheat Engine 7.4","Lua"}; //TUDO QUE TIVER NESSA LISTA VAI SER BARRADO PELO SYSTEM
    int i=0;

    while(i<=2){
        HWND janelaDetect = FindWindow(NULL,appsIlicitos[i]);
        if(janelaDetect!=NULL){
            cout << "App ilicito aberto no seu pc, nome: " << appsIlicitos[i] << endl;
            Sleep(2000);
            system("cls");
        }else{
            cout << "Nada encontrado ate o momento..." << endl;
            Sleep(2000);
            system("cls");
            if(janelaDetect==NULL){
                i++;
                if(i==2){
                    i=0;
                }
            }
        }
    }

    return 0;
}
