# JogoDaVelha
Trabalho Acadêmico feito por mim, no primeiro semestre do curso Análise e Desenvolvimento de Sistemas
namespace JOGOVELHA
{
    class Program
    {
        static void Main(string[] args)
        {
            //ALUNO: FELIPE TORRES GONTIJO

            string jogador1 = ""; // nome do jogador
            string jogador2 = ""; // nome do jogador
            bool executa = true; //estrutura de repetição da tabela
            string pos = ""; // variavel que valida as posições
            //double turno = 5; // var que auxilia rodadas do jogo para ter vencedores
            bool cont = true;

            //tabela do jogo
            string p1 = "1", p2 = "2", p3 = "3";
            string p4 = "4", p5 = "5", p6 = "6";
            string p7 = "7", p8 = "8", p9 = "9";

            Console.WriteLine("=============== JOGO DA VELHA ===============");
            Console.WriteLine("\n\nVamos começar uma partida. Informe o nome dos jogadores");
            Console.Write("\n\nNome do jogador 1: "); //recolhe inf do nome do jogador
            jogador1 = Console.ReadLine();

            Console.Write("Nome do jogador 2: "); //recolhe inf do nome do jogador
            jogador2 = Console.ReadLine();

            Console.Clear();

            //começa o jogo
            while (executa) // executa enquanto for vdd, assim que alguem vencer executa = false
            {
               // for (double i = 0; i <= turno - 1; i++)  // caso não houver vencedores neste periodo o jogo é empate
                {
                    Console.WriteLine("============= JOGO DA VELHA =============\n\n");
                    Console.WriteLine("\t       |       |        ");
                    Console.WriteLine("\t   " + p1 + "   |   " + p2 + "   |   " + p3 + "    ");
                    Console.WriteLine("\t-------|-------|------- ");
                    Console.WriteLine("\t   " + p4 + "   |   " + p5 + "   |   " + p6 + "    ");
                    Console.WriteLine("\t-------|-------|------- ");
                    Console.WriteLine("\t   " + p7 + "   |   " + p8 + "   |   " + p9 + "    ");
                    Console.WriteLine("\t       |       |        ");

                    pos = player1(jogador1); //função para as ações do jogador 1

                    Console.Clear();

                    while (cont)
                    { 
                        //ifs de subs de posição do jogador 1, e em caso de escolher posição já selecionada.
                        if (pos == "1")
                        {
                            if (p1 == "1")
                            {
                                p1 = "X";
                                cont = false;
                            }
                            else if (p1 == "X" || p1 == "O")
                            {
                                Console.WriteLine("Numero ja foi selecionado por outro jogador anteriormente. Tente denovo.");
                                pos = player1(jogador1);
                            }
                        }

                        else if (pos == "2")
                        {
                            if (p2 == "2")
                            {
                                p2 = "X";
                                cont = false;
                            }
                            else if (p2 == "X" || p2 == "O")
                            {
                                Console.WriteLine("Numero ja foi selecionado por outro jogador anteriormente. Tente denovo.");
                                pos = player1(jogador1);
                            }
                        }

                        else if (pos == "3")
                        {
                            if (p3 == "3")
                            {
                                p3 = "X";
                                cont = false;
                            }
                            else if (p3 == "X" || p3 == "O")
                            {
                                Console.WriteLine("Numero ja foi selecionado por outro jogador anteriormente. Tente denovo.");
                                pos = player1(jogador1);
                            }
                        }


                        else if (pos == "4")
                        {
                            if (p4 == "4")
                            {
                                p4 = "X";
                                cont = false;
                            }
                            else if (p4 == "X" || p4 == "O")
                            {
                                Console.WriteLine("Numero ja foi selecionado por outro jogador anteriormente. Tente denovo.");
                                pos = player1(jogador1);
                            }
                        }

                        else if (pos == "5")
                        {
                            if (p5 == "5")
                            {
                                p5 = "X";
                                cont = false;
                            }
                            else if (p5 == "X" || p5 == "O")
                            {
                                Console.WriteLine("Numero ja foi selecionado por outro jogador anteriormente. Tente denovo.");
                                pos = player1(jogador1);
                            }
                        }

                        else if (pos == "6")
                        {
                            if (p6 == "6")
                            {
                                p6 = "X";
                                cont = false;
                            }
                            else if (p6 == "X" || p6 == "O")
                            {
                                Console.WriteLine("Numero ja foi selecionado por outro jogador anteriormente. Tente denovo.");
                                pos = player1(jogador1);
                            }
                        }

                        else if (pos == "7")
                        {
                            if (p7 == "7")
                            {
                                p7 = "X";
                                cont = false;
                            }
                            else if (p7 == "X" || p7 == "O")
                            {
                                Console.WriteLine("Numero ja foi selecionado por outro jogador anteriormente. Tente denovo.");
                                pos = player1(jogador1);
                            }
                        }

                        else if (pos == "8")
                        {
                            if (p8 == "8")
                            {
                                p8 = "X";
                                cont = false;
                            }
                            else if (p8 == "X" || p8 == "O")
                            {
                                Console.WriteLine("Numero ja foi selecionado por outro jogador anteriormente. Tente denovo.");
                                pos = player1(jogador1);
                            }
                        }

                        else if (pos == "9")
                        {
                            if (p9 == "9")
                            {
                                p9 = "X";
                                cont = false;
                            }
                            else if (p9 == "X" || p9 == "O")
                            {
                                Console.WriteLine("Numero ja foi selecionado por outro jogador anteriormente. Tente denovo.");
                                pos = player1(jogador1);
                            }

                        }
                    }

                    cont = true;

                    //ifs em caso de vitria (fim de jogo) - jogador 1
                    if (p1 == "X" && p2 == "X" && p3 == "X")
                    {
                        Console.WriteLine(jogador1 + ", venceu!! Parabéns");
                        Console.ReadLine();
                        executa = false;
                        break;
                    }
                    else if (p4 == "X" && p5 == "X" && p6 == "X")
                    {
                        Console.WriteLine(jogador1 + ", venceu!! Parabéns");
                        Console.ReadLine();
                        executa = false;
                        break;
                    }
                    else if (p7 == "X" && p8 == "X" && p9 == "X")
                    {
                        Console.WriteLine(jogador1 + ", venceu!! Parabéns");
                        Console.ReadLine();
                        executa = false;
                        break;
                    }
                    else if (p1 == "X" && p5 == "X" && p9 == "X")
                    {
                        Console.WriteLine(jogador1 + ", venceu!! Parabéns");
                        Console.ReadLine();
                        executa = false;
                        break;
                    }
                    else if (p3 == "X" && p5 == "X" && p7 == "X")
                    {
                        Console.WriteLine(jogador1 + ", venceu!! Parabéns");
                        Console.ReadLine();
                        executa = false;
                        break;
                    }
                    else if (p1 == "X" && p4 == "X" && p7 == "X")
                    {
                        Console.WriteLine(jogador1 + ", venceu!! Parabéns");
                        Console.ReadLine();
                        executa = false;
                        break;
                    }
                    else if (p2 == "X" && p5 == "X" && p8 == "X")
                    {
                        Console.WriteLine(jogador1 + ", venceu!! Parabéns");
                        Console.ReadLine();
                        executa = false;
                        break;
                    }
                    else if (p3 == "X" && p6 == "X" && p9 == "X")
                    {
                        Console.WriteLine(jogador1 + ", venceu!! Parabéns");
                        Console.ReadLine();
                        executa = false;
                        break;
                    }

                    Console.Clear();

                    if ((p1 == "X" || p1 == "O") && (p2 == "X" || p2 == "O") && (p3 == "X" || p3 == "O") && (p4 == "X" || p4 == "O") && (p5 == "X" || p5 == "O") && (p6 == "X" || p6 == "O") && (p7 == "X" || p7 == "O") && (p8 == "X" || p8 == "O") && (p9 == "X" || p9 == "O")) 
                    {
                        executa = false;
                        Console.WriteLine("O jogo terminou empatado, ou seja, deu VELHA! Execute novamente, e tente vencer seu oponente!");
                        Console.ReadLine();
                        break;
                    }

                    Console.WriteLine("============= JOGO DA VELHA =============\n\n");
                    Console.WriteLine("\t       |       |        ");
                    Console.WriteLine("\t   " + p1 + "   |   " + p2 + "   |   " + p3 + "    ");
                    Console.WriteLine("\t-------|-------|------- ");
                    Console.WriteLine("\t   " + p4 + "   |   " + p5 + "   |   " + p6 + "    ");
                    Console.WriteLine("\t-------|-------|------- ");
                    Console.WriteLine("\t   " + p7 + "   |   " + p8 + "   |   " + p9 + "    ");
                    Console.WriteLine("\t       |       |        ");

                    pos = player2(jogador2); //função para ações do jogador 2

                    Console.Clear();

                    while (cont)
                    {
                        //ifs de subs de posição do jogador 1, e em caso de escolher posição já selecionada.
                        if (pos == "1")
                        {
                            if (p1 == "1")
                            {
                                p1 = "O";
                                cont = false;
                            }
                            else if (p1 == "X" || p1 == "O")
                            {
                                Console.WriteLine("Numero ja foi selecionado por outro jogador anteriormente. Tente denovo.");
                                pos = player2(jogador2);
                            }
                        }

                        else if (pos == "2")
                        {
                            if (p2 == "2")
                            {
                                p2 = "O";
                                cont = false;
                            }
                            else if (p2 == "X" || p2 == "O")
                            {
                                Console.WriteLine("Numero ja foi selecionado por outro jogador anteriormente. Tente denovo.");
                                pos = player2(jogador2);
                            }
                        }

                        else if (pos == "3")
                        {
                            if (p3 == "3")
                            {
                                p3 = "O";
                                cont = false;
                            }
                            else if (p3 == "X" || p3 == "O")
                            {
                                Console.WriteLine("Numero ja foi selecionado por outro jogador anteriormente. Tente denovo.");
                                pos = player2(jogador2);
                            }
                        }


                        else if (pos == "4")
                        {
                            if (p4 == "4")
                            {
                                p4 = "O";
                                cont = false;
                            }
                            else if (p4 == "X" || p4 == "O")
                            {
                                Console.WriteLine("Numero ja foi selecionado por outro jogador anteriormente. Tente denovo.");
                                pos = player2(jogador2);
                            }
                        }

                        else if (pos == "5")
                        {
                            if (p5 == "5")
                            {
                                p5 = "O";
                                cont = false;
                            }
                            else if (p5 == "X" || p5 == "O")
                            {
                                Console.WriteLine("Numero ja foi selecionado por outro jogador anteriormente. Tente denovo.");
                                pos = player2(jogador2);
                            }
                        }

                        else if (pos == "6")
                        {
                            if (p6 == "6")
                            {
                                p6 = "O";
                                cont = false;
                            }
                            else if (p6 == "X" || p6 == "O")
                            {
                                Console.WriteLine("Numero ja foi selecionado por outro jogador anteriormente. Tente denovo.");
                                pos = player2(jogador2);
                            }
                        }

                        else if (pos == "7")
                        {
                            if (p7 == "7")
                            {
                                p7 = "O";
                                cont = false;
                            }
                            else if (p7 == "X" || p7 == "O")
                            {
                                Console.WriteLine("Numero ja foi selecionado por outro jogador anteriormente. Tente denovo.");
                                pos = player2(jogador2);
                            }
                        }

                        else if (pos == "8")
                        {
                            if (p8 == "8")
                            {
                                p8 = "O";
                                cont = false;
                            }
                            else if (p8 == "X" || p8 == "O")
                            {
                                Console.WriteLine("Numero ja foi selecionado por outro jogador anteriormente. Tente denovo.");
                                pos = player2(jogador2);
                            }
                        }

                        else if (pos == "9")
                        {
                            if (p9 == "9")
                            {
                                p9 = "O";
                                cont = false;
                            }
                            else if (p9 == "X" || p9 == "O")
                            {
                                Console.WriteLine("Numero ja foi selecionado por outro jogador anteriormente. Tente denovo.");
                                pos = player2(jogador2);
                            }
                        }
                    }
                    cont = true;

                    //ifs em caso de vitoria (fim de jogo) - jogador 2
                    if (p1 == "O" && p2 == "O" && p3 == "O")
                    {
                        Console.WriteLine(jogador2 + ", venceu!! Parabéns");
                        Console.ReadLine();
                        executa = false;
                        break;
                    }
                    else if (p4 == "O" && p5 == "O" && p6 == "O")
                    {
                        Console.WriteLine(jogador2 + ", venceu!! Parabéns");
                        Console.ReadLine();
                        executa = false;
                        break;
                    }
                    else if (p7 == "O" && p8 == "O" && p9 == "O")
                    {
                        Console.WriteLine(jogador2 + ", venceu!! Parabéns");
                        Console.ReadLine();
                        executa = false;
                        break;
                    }
                    else if (p1 == "O" && p5 == "O" && p9 == "O")
                    {
                        Console.WriteLine(jogador2 + ", venceu!! Parabéns");
                        Console.ReadLine();
                        executa = false;
                        break;
                    }
                    else if (p3 == "O" && p5 == "O" && p7 == "O")
                    {
                        Console.WriteLine(jogador2 + ", venceu!! Parabéns");
                        Console.ReadLine();
                        executa = false;
                        break;
                    }
                    else if (p1 == "O" && p4 == "O" && p7 == "O")
                    {
                        Console.WriteLine(jogador2 + ", venceu!! Parabéns");
                        Console.ReadLine();
                        executa = false;
                        break;
                    }
                    else if (p2 == "O" && p5 == "O" && p8 == "O")
                    {
                        Console.WriteLine(jogador2 + ", venceu!! Parabéns");
                        Console.ReadLine();
                        executa = false;
                        break;
                    }
                    else if (p3 == "O" && p6 == "O" && p9 == "O")
                    {
                        Console.WriteLine(jogador2 + ", venceu!! Parabéns");
                        Console.ReadLine();
                        executa = false;
                        break;
                    }
                }
            }
        }
            static string player1(string jogador1)
            {
            string subs = ""; // variavel que valida as posições
            int aux = 0;
            bool cont = true;

                Console.Write("\n\n" + jogador1 + ", escolha sua posição: ");
                aux = Convert.ToInt32(Console.ReadLine());

            while (cont)
            {
                    if (aux <= 9 && aux >= 1)
                    {
                        subs = aux.ToString();
                        cont = false;
                    }
                    else
                    {
                    Console.WriteLine("\n" + jogador1 + " posição na qual informou não foi valida, tente novamente");
                    Console.Write("Qual posição deseja escolher?");
                    aux = Convert.ToInt32(Console.ReadLine());
                    Console.Clear();
                }
            }
            return subs;
            }

            static string player2(string jogador2)
        {
            string subs = ""; // variavel que valida as posições
            int aux = 0;
            bool cont = true;

            Console.Write("\n\n" + jogador2 + ", escolha sua posição: ");
            aux = Convert.ToInt32(Console.ReadLine());

            while (cont)
            {
                if (aux <= 9 && aux >= 1)
                {
                    subs = aux.ToString();
                    cont = false;
                }
                else
                {
                    Console.WriteLine("\n" + jogador2 + " posição na qual informou não foi valida, tente novamente");
                    Console.Write("Qual posição deseja escolher?");
                    aux = Convert.ToInt32(Console.ReadLine());
                    Console.Clear();
                }
            }
            return subs;
        }
    }
}
