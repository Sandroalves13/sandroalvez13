# sandroalvez13
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
