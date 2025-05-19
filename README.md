# ATV_FOR_CJ3027317

int valor = 1;
for (; valor != 0;)
{
    Console.WriteLine("-------MENU-------");
    Console.WriteLine("0 - sair");
    Console.WriteLine("1 - exercício 1");
    Console.WriteLine("2 - exercício 2");
    Console.WriteLine("3 - exercício 3");
    Console.WriteLine("4 - exercício 4");
    Console.WriteLine("5 - exercício 5");
    Console.WriteLine("6 - exercício 6");
    Console.WriteLine("7 - exercício 7\n\n\n");
    valor = int.Parse(Console.ReadLine());

    switch (valor)
    {
        case 0:
            Console.Clear();
            Console.WriteLine("Obrigada por usar o sistema!");
            break;




        case 1:
            Console.Clear();
            Console.WriteLine("Ler e Imprimir todos os números de 1 até valor inserido pelo usuário.\n\n");
            Console.WriteLine("Digite um número y qualquer:");
            int y = int.Parse(Console.ReadLine());
            int x = 1;
            Console.Clear();

            if (y < x)
            {
                (x, y) = (y, x);
            }
            for (int i = x; i <= y; i++)
            {
                Console.WriteLine($"\n{i}\n");
            }
            break;


        case 2:
            Console.Clear();
            Console.WriteLine("Ler e Imprimir todos os números pares de 1 até valor inserido pelo usuário.\n\n");
            Console.WriteLine("Digite um número b qualquer:");
            int b = int.Parse(Console.ReadLine());
            int a = 1;
            Console.Clear();

            if (b < a)
            {
                (a, b) = (b, a);
            }
            for (int i = a; i <= b; i++)
            {
                if (i % 2 == 0)
                {
                    Console.WriteLine($"\n{i}\n");
                }

            }
            break;

        case 3:
            Console.Clear();
            Console.WriteLine("Ler e Imprimir todos os números pares de 1000 até valor inserido pelo usuário>\n\n");
            Console.WriteLine("Digite um número z qualquer:");
            int z = int.Parse(Console.ReadLine());
            Console.Clear();

            for (int i = 1000; i >= z; i--)
            {
                if (i % 2 == 0)
                    Console.WriteLine($"\n{i}\n");
            }
            break;


        case 4:
            Console.Clear();
            Console.WriteLine("Soma dos números positivos:\n\n");
            int soma = 0;

            for (int i = 0; soma < 200; i++)
            {
                Console.WriteLine("Digite um valor qualquer:");
                int w = int.Parse(Console.ReadLine());
                if (w > 0)
                {
                    Console.WriteLine(w);
                    soma += w;
                }
                Console.WriteLine($"A soma é {soma}\n\n");
               
            }

            break;


        case 5:
            Console.Clear();
            Console.WriteLine("Divisores de um número:\n\n");
            Console.WriteLine("Digite um número qualquer:\n");
            int numero = int.Parse(Console.ReadLine());
            Console.Clear();

            for (int i = 1; i <= numero; i++)
            {
                if (numero % i == 0)
                {
                    Console.WriteLine($"\n{i}\n");
                }
            }
            break;


        case 6:
            Console.Clear();
            Console.WriteLine("Maior e menor entre 10 números:\n\n");
            Console.WriteLine("Digite o número: ");
            int aleatorio = int.Parse(Console.ReadLine());
            int maior = aleatorio;
            int menor = aleatorio;
            Console.Clear();

            for(int i = 1; i < 10; i++)
            {
                Console.WriteLine("Digite o número: ");
              aleatorio = int.Parse(Console.ReadLine());
           
                
                if (aleatorio > maior)  maior = aleatorio;
                
                if (aleatorio < menor)  menor = aleatorio;
                
              
            }
            Console.WriteLine($"O maior número é {maior}");
            Console.WriteLine($"O menor número é {menor}");

            break;


        case 7:
            Console.Clear();
            Console.WriteLine("Soma de Ímpares e Pares enquanto não for digitado zero:\n\n");
            int somaP = 0;
            int somaI = 0;
            int qualquer = 1;
            Console.Clear();

            for (; qualquer != 0;)
            {
                Console.WriteLine("Digite um número qualquer:\n");
                qualquer = int.Parse(Console.ReadLine());

                if (qualquer % 2 == 0)
                {
                    somaP += qualquer;
                }
                else
                {
                    somaI += qualquer;
                }
                Console.WriteLine($"\nA soma dos pares é {somaP}\n");
                Console.WriteLine($"A soma dos ímpares é {somaI}\n");
            }

            break;


        default:
            Console.Clear();
            Console.WriteLine("Opção Inválida!");
            break;
    }
}

