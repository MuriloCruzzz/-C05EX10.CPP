#include <iostream>
#include <iomanip>
#include <ctime> //
using namespace std;

int main(void)
{

  struct tm *PHORA, * PUNIVERS, TEMPO; // estrutura que contem varios tipos de dados
  time_t AGORA, MOMENTO; // tipo de dado derivado não primitivo

  AGORA = time(NULL);
  PHORA = localtime(&AGORA);
  PUNIVERS = gmtime(&AGORA);

  TEMPO.tm_year = 2003-1900;
  TEMPO.tm_mon  = 6-1;
  TEMPO.tm_mday = 1;
  TEMPO.tm_hour = 17;
  TEMPO.tm_min  = 45;
  TEMPO.tm_sec  = 34;
  MOMENTO = mktime(&TEMPO);

  cout << "Data/Hora: " << asctime(PHORA) << endl;
  cout << "Data/Hora: " << ctime(&AGORA) << endl;
  cout << "Hora e Data universais..: ";
  cout << asctime(PUNIVERS) << endl;
  cout << "--> 01/06/2002 17:45:34: ";
  cout << ctime(&MOMENTO) << endl;

  cout << "Tecle <Enter> para encerrar... ";
  cin.get();
  return 0;
}
