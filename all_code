#include<iostream>
#include<fstream>
#include <windows.h>
#include<string>
#include<conio.h>

            #ifdef __cplusplus__
            #include <cstdlib>
            #else
            #include <stdlib.h>
            #endif

//  system ("color 0a");
using namespace std;

void z() {Sleep(100);}
void z2() {Sleep(210);}
void z3() {Sleep(900);}
void clearscreen(){for(int i=0;i<100;i++){cout<<"";}}

class Murdock{
   private:
      int stamina=20;
      int inpoints=0;
      
   public:
      
      //Murdock(){ //constructor
         
      //}
      void set_stamina(int stamina2){
         stamina=stamina2;
      }
      
      void set_inpoints(int intelligence){
         inpoints=intelligence;
      }
      
      int get_stamina(){
         return stamina;
      }
      
      int get_inpoints(){
         return inpoints;
      }
      
      void mod_intelligence(int more){
         int inte=get_inpoints();
         
         inte=inte+more;
         
         set_inpoints(inte);
      }
      
      void mod_stamina(int type){
         int stam;
         stam=get_stamina();
         
         if(type==1){ //take away
            stam=stam-2;
         }
         else if(type==2){ //give back
            stam=stam+2;     
         }
         set_stamina(stam);
      }
      
      
      void blink(){
         int in;
         in=get_stamina();
         if(in<=0){
            cout<<"not enough stamina!! eat something";
            z3();
         }
         else{
            string murdy="(^.w.^)";
            string murdy2="(^owo^)";
         
         for(int i=0;i<6;i++){
            cout<<murdy;
            z();
            if (system("CLS")) system("clear");
            z();
            cout<<" ";
            cout<<murdy2;
            z2();
            if (system("CLS")) system("clear");
            cout<<" ";
            
         }
         mod_stamina(1);
         }
      }
      
      void run(){
         string murdy="(^.w.^)";
         int st;
         st=get_stamina();
         if(st<=0){
            cout<<"not enough stamina!! eat something";
            z3();
         }
         else{
            for(int i=0;i<8;i++){
               cout<<"    ";
               z();
               for(int j=0;j<i;j++){
                  cout<<murdy;
                  z();
                  if (system("CLS")) system("clear");
               }
            }
            mod_stamina(1);
         }
      }
      
      void surprised(){
         string murdy="(^.w.^)";
         string murdy2="(^owo^)";
         
         for(int i=0;i<6;i++){
            cout<<murdy;
            z();
            if (system("CLS")) system("clear");
            z();
            cout<<" ";
            cout<<murdy2;
            z2();
            if (system("CLS")) system("clear");
            cout<<" ";
            
         }
      }
      
      void eating(){
         string murdy="(^.w.^) ***";
         string murdy2="(^.0.^)  **";
         string murdy3="(^.w.^)   *";
         
         for(int i=0;i<6;i++){
            cout<<murdy;
            z2();
            z2();
            if (system("CLS")) system("clear");
            z();
            cout<<" ";
            cout<<murdy2;
            z2();
            z2();
            if (system("CLS")) system("clear");
            cout<<" ";
            cout<<murdy3;
            z2();
            z2();
            if (system("CLS")) system("clear");
            cout<<" ";
            
         }     
          mod_stamina(2);    
      }
         
         void chat(string yousay){
            //string yousay
            string kittysay="meow\n";
            string kittysay2="prrrrr\n";
            string kittysay3="meeeeow prrr\n";
            
            int count=0;
            
            //kitty replies
            while(yousay!="bye"){
               cin>>yousay;
               int value=rand()%100;
               if(value<25){
                  cout<<kittysay2;
               }
               else if(value>25&&value<50){
                  cout<<kittysay3;
               }
               else if(value<100&&value>50){
                  cout<<kittysay;
               }
               else{
                  cout<<kittysay;
               }
               if(yousay=="hey"){
                  cout<<"prrrr mee!!\n";
               }
               if(yousay=="cute"){
                  cout<<">w< meeeow...\n";
               }
               if(yousay=="sweetie"){
                  Murdock gatito;
                  gatito.surprised();
               }
               count++;
            }
            mod_intelligence(count);
         }

         void math(){
            string murdy="(^.3.^)- <( ";
            int reply;
            int intelligence=0;
            
            cout<<"let's start, when you wanna end just write -1\n\n";
            
            while(reply!=-1){
               int value=rand()%100;
               int value2=rand()%100;
               cout<<murdy;
               cout<<value<<" + ";
               cout<<value2<<" ? ";
               cout<<" )\n";
            
               cin>>reply;
               if(reply==(value+value2)){
                  cout<<"meow!\n";
                  cout<<"+1 point of intelligence\n";
                  intelligence++;
                  intelligence++;
               }
               else{
                  cout<<"meow... (^u__u^)\n";
               }
            
            }
            
            mod_intelligence(intelligence);
         }
   
};

int main(){
   system ("color 0a");
   Murdock gatito;
   int ans;
   string ans1;
   int suma;
   
   
   //gatito.blink();
   //gatito.run();
   //gatito.surprised();
   //gatito.eating();
   //gatito.chat(ans1);
   //gatito.math();
   

   while(ans!=0){
      
   cout<<"\n\n\n what you wanna little Murdock to do?\n\n0-exit\n1-blink\n2-do excersice\n3-eat\n4-chat with him\n5-do math with him\n6-see stamina\n7-see intelligence\n";
   cout<<"your option: ";
   cin>>ans;

   switch(ans){
      case 1:
         gatito.blink();
         break;
      case 2:
         gatito.run();
         break;
      case 3:
         gatito.eating();
         break;
      case 4:{
         string ans3;
         cout<<"write your text now:\n";
         gatito.chat(ans3);
         break;
         }
      case 5:
         gatito.math();
         break;
      case 6:{
         int st;
      	st=gatito.get_stamina();
      	cout<<st<<"\n";
      	z3();
         break;
      }

      case 7:{
      	int in;
         in=gatito.get_inpoints();
         cout<<in<<"\n";
         z3();
         break;
      }
         
      default:
         cout<<"invalid action please try again\n";
         break;
   } //end switch case
      if (system("CLS")) system("clear");
   } //exit
   
   

  
   
   
}
