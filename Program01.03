using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace practica_01_03
{
    internal class Program
    {
        static void Main(string[] args)
        {
            //CalendarioEntrada cumpleaños = new CalendarioEntrada();
            //cumpleaños.Dia = "sunday";
            //Console.WriteLine(cumpleaños.Date);

            //Console.ReadLine();

            CalendarioEntrada hb = new CalendarioEntrada();
            Console.WriteLine(hb.Date);


        }

    }

    public class CalendarioEntrada
    {
        public DateTime Fecha;

        public DateTime Date
        {
            get { return Fecha; }
            set
            {
                if (value.Year > 1990 && value.Year <= DateTime.Today.Year)
                {
                    Fecha = value;
                }
                else
                {
                    throw new ArgumentOutOfRangeException("Fecha");
                }
            }
        }

        //public string Dia;


        public void setFecha( string fechaString)
        {
            DateTime dt = Convert.ToDateTime(fechaString);
            if(dt.Year > 1990 && dt.Year <= DateTime.Today.Year)
            {
                Fecha = dt;
            }
            else
            {
                throw new ArgumentOutOfRangeException("fechaString");
            }
        }

        public TimeSpan GetTimeSpan(string fechaString)
        {
            DateTime dt = Convert.ToDateTime(fechaString);
            if(dt.Ticks<Fecha.Ticks)
            {
                return Fecha - dt;
            }
            else
            {
                throw new ArgumentOutOfRangeException("fechaString");
            }
        }
    }

    public class CalendarioInicializado
    {
        public string Dia = "Monday";
    }
}
