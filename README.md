[Patika.dev](https://github.com/mordulu)


Dosyalarımın içinde yer alan program.cs'ye girilme zahmeti olmaması adına aşağıya çalışmamı önizleme olarak ekliyorum(süslü parantezler önizlemede hata verdiğinden konumlandırmalarına dikkat etmeyiniz)


# C-101-Hata-Yonetimi Ders Notları

             using System;

              namespace operatorler

              {

              class Program
              {
    
                 static void Main(string[] args)
              {
              //      try
              //        {
               //           Console.WriteLine("Bir sayi giriniz:");
               //           int sayi = Convert.ToInt32(Console.ReadLine());
               //
               //            Console.WriteLine("Girmiş olduğunuz sayi :" + sayi);
               //        }
               //        catch(Exception ex)
               //        {
               //           Console.WriteLine("Hata: "+ ex.Message.ToString());
               //        }
               // finally   
               //  {

               //    Console.WriteLine("İşlem tamamlandı");  
               //}
           try
           {
              //  int a = int.Parse("test");
                int a = int.Parse("-20000000000");
           }
           catch (ArgumentException ex)
           {
            Console.WriteLine ("Boş değer girdiniz");
            Console.WriteLine(ex);
           }  
             catch(FormatException ex)
           {
            Console.WriteLine ("Veri tipi uygun değil");
            Console.WriteLine(ex);

           }
            catch(OverflowException ex)
            {
               Console.WriteLine("Çok küçük yada çok büyük bir değer girdiniz.");
               Console.WriteLine(ex);
         

            }
            finally{
               Console.WriteLine("İşlem başarıyla tamamlandı.");
            }
            }
            }         
            }
