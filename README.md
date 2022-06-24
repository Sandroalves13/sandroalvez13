
O sistema tem como base três sensores e dois atuadores que estão denominados S1 e S2, esse são responsáveis para acionar o braço mecânico, que está para verificar as peças, Grandes (Alta) e pequenas (baixa), assim atuando como um separador de peças
•	S1 – Peças correta, deste que esta esteja no seu local encontrando S2
•	S2 – Liga o Soprador para descarte das peças


Modo construtivo do sistema


•	Esteira inicia com o comando Liga
•	Sopradores são acionados para descarte das peças
•	Atuadores S1 e S2 fazem o filtro das peças
•	Espera o tempo e retorna o inicio 

segue o códif para verificar conforme descrição acima


aplicativo desenvolvido via labview, para controle de peças
const int Bliga=2;
const int Bdesligado=4;
int ligado;
int desligado;
const int k=5;
int liga;
int desliga;

void Setup ()
{
  pinMode (Bliga,INPUT); 
  pinMode (Bdesligado, INPUT);
  pinMode (k,OUTPUT);
  liga=0;
  desligado=0; 
}
void Loop () {
  desligado==digitalRead (Bdesligado);
  if(desligado==LOW);
     desligado=1;
     if (desligado==1) {digitalWrite(k,LOW);
                      liga=0;}
      ligado=digitalRead (Bliga);
      if(ligado==HIGH){
        ligado-0;
        if(liga==1){digitalWrite (k,HIGH);
        desliga=0;
      }}}
