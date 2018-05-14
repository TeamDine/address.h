# address.h
///Cabecera de la clase address 
#ifndef ADDRESS_H_INCLUDED
#define ADDRESS_H_INCLUDED

/*** Cabeceras del sistema ***/
#include <string>

class Address{
    private:
        std::string mainStreet;     ///Calle principal
        std::string numExt;         ///Numero exterior
        std::string numInt;         ///Numero interior
        std::string suburb;         ///Colonia
        std::string country;        ///Ciudad

    public:
        Address();             ///Constructor base
        Address(const Address&);  /// Constructor Copia
        Address(const std::string&, std::string&, std::string&, std::string&, std::string& );  ///Constructor Parametrizado

        /*** getters ***/
        std::string getMainStreet();
        std::string getNumExt();
        std::string getNumInt();
        std::string getSuburb();
        std::string getCountry();

        /*** setters ***/
        void setMainStreet(const std::string&);
        void setNumExt(const std::string&);
        void setNumInt(const std::string&);
        void setSuburb(const std::string&);
        void setCountry(const std::string&);

        std::string toString();     ///Imprime direccion completa

};

#endif // ADDRESS_H_INCLUDED
