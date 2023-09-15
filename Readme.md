Algoritmo "Lanchonete Icaro"
var

  opc, oplanch, opbebida     : inteiro
  opacompanhamento, qtd      : inteiro
  vltotal, vllanch           : real
  vlbebida, vlacompanhamento : real
  lancheS, bebidas           : real
  acompanhamentos, toTal     : real
Inicio
   Repita

     vllanch  := 0
     vlbebida := 0
     vlacompanhamento := 0

      Escreval (" MENU ICARO ")
      Escreval (" 1 Lanche           ")
      Escreval (" 2 Bebidas          ")
      Escreval (" 3 Acopanhamentos   ")
      Escreval (" 0 finalizar pedido ")
      Escreval  (" Faça Seu pedido   ")
      escreval (" Escolha uma opção  ")
      Leia (opc)
      escolha opc

      caso 1
         Repita
            Escreval (" LANCHES ")
            Escreval (" 1 x-burger -> R$ 10,00")
            Escreval (" 2 X-Salada -> R$ 12,00")
            Escreval (" 3 X-Bacon  -> R$ 14.00")
            Escreval (" 4 X-Tudo -> R$ 18.00")
            Escreval (" 5 Vegetariano -> R$ 10.00")
            Escreval (" 6 Cheeseburguer -> R$ 9.00")
            Escreval (" 7 Duplo -> R$ 16.00")
            Escreval (" 0 Voltar ao menu anterior "  )
            Escreval (" Escolha uma opção de lanche "  )
            leia(oplanch)

            Se oplanch = 0 então
               interrompa
            Fimse

            Escreval ("Informe a quantidade")
            Leia (qtd)

            Se oplanch = 1 então
               vllanch <- vllanch + 10 * qtd
            Senao
               Se oplanch = 2 então
                  vllanch <- vllanch + 12 * qtd
               Senao
                  Se oplanch = 3 então
                     vllanch <- vllanch + 14 * qtd
                  Senao
                     Se oplanch = 4 então
                        vllanch <- vllanch + 18 * qtd
                     Senao
                        Se oplanch = 5 então
                           vllanch <- vllanch + 10 * qtd
                        Senao
                           Se oplanch = 6 então
                              vllanch <- vllanch + 9 * qtd
                           Senao
                              Se oplanch = 7 então
                                 vllanch <- vllanch + 16 * qtd
                              Fimse
                           Fimse
                        Fimse
                     Fimse
                  Fimse
               Fimse
            Fimse
         Ate oplanch = 0
         Escreval("...................................")
         Escreval("")
         Escreval("valor Do Pedido = R$", vllanch,",00")
         Escreval("...................................")
        lanches := lanches + vllanch
        Timer 3000
        Timer 0
      caso 2
         Repita
            Escreval (" BEBIDAS ")
            Escreval (" 1 Refrigerante -> R$  5,00")
            Escreval (" 2 Suco Natural -> R$  4,00")
            Escreval (" 3 Suco Artificial -> R$  2,00")
            Escreval (" 4 Agua -> R$  3,00")
            Escreval (" 5 Agua Gaseificada -> R$  5,00")
            Escreval (" 6 Cafe Gelado -> R$  9.00")
            Escreval (" 7 Milk Shake -> R$ 12,00")
            Escreval (" 0 Voltar ao menu anterior "           )
            Escreval (" Escolha uma opção de bebida "         )
            leia   ( opbebida)

            Se opbebida = 0 então
               interrompa
            Fimse

            Escreval (" Informe a Quantidade ")
            leia     ( qtd )

            Se opbebida = 1 então
               vlbebida <- vlbebida + 5 * qtd
            Senao
               Se opbebida = 2 então
                  vlbebida <- vlbebida + 4 * qtd
               Senao
                  Se opbebida = 3 então
                     vlbebida <- vlbebida + 2 * qtd
                  Senao
                     Se opbebida = 4 então
                        vlbebida <- vlbebida + 3 * qtd
                     Senao
                        Se opbebida = 5 então
                           vlbebida <- vlbebida + 5 * qtd
                        Senao
                           Se opbebida = 6  então
                              vlbebida <- vlbebida + 9 * qtd
                           Senao
                              Se opbebida = 7 então
                                 vlbebida <- vlbebida + 12 * qtd
                              Fimse
                           Fimse
                        Fimse
                     Fimse
                  Fimse
               Fimse
            Fimse
         Ate opbebida = 0
         Escreval("....................................")
         Escreval("")
         Escreval("valor Do Pedido = R$", vlbebida,",00")
         Escreval("....................................")
        bebidas := bebidas + vlbebida
        Timer 3000
        Timer 0
      caso 3
         Repita
            Escreval (" ACOMPANHAMENTOS ")
            Escreval (" 1 Batata Frita -> R$ 8,00 ")
            Escreval (" 2 Salada -> R$ 12,50 ")
            Escreval (" 3 Aneis de Cebola -> R$ 14,00 ")
            Escreval (" 4 Batata Doce Frita -> R$ 9,00 ")
            Escreval (" 5 Nuggets -> R$10,00 ")
            Escreval (" 6 Coxinha -> R$ 5,00 ")
            Escreval (" 7 Polenta Frita -> R$ 13,00 ")
            Escreval (" Escolha uma opção de acompnhamento  ")
            leia(opacompanhamento)


            Se opacompanhamento = 0 então
               interrompa
            Fimse

            Escreval ("Informe a quantidade")
            Leia (qtd)

            Se opacompanhamento = 1 então
               vlacompanhamento <- vlacompanhamento + 8 * qtd
            Senao
               Se opacompanhamento = 2 então
                  vlacompanhamento <- vlacompanhamento + 12,50 * qtd
               Senao
                  Se opacompanhamento = 3 então
                     vlacompanhamento <- vlacompanhamento + 14 * qtd
                  Senao
                     Se opacompanhamento = 4 então
                        vlacompanhamento <- vlacompanhamento + 9 * qtd
                     Senao
                        Se opacompanhamento = 5 então
                           vlacompanhamento <- vlacompanhamento + 10 * qtd
                        Senao
                           Se opacompanhamento = 6 então
                              vlacompanhamento <- vlacompanhamento + 5 * qtd
                           Senao
                              Se opacompanhamento = 7 então
                                 vlacompanhamento <- vlacompanhamento + 13 * qtd
                              Fimse
                           Fimse
                        Fimse
                     Fimse
                  Fimse
               Fimse
            Fimse
         Ate opacompanhamento = 0
         Escreval("valor Do Pedido = R$", vlacompanhamento,",00")
        acompanhamentos := acompanhamentos + vlacompanhamento
        Timer 3000
        Timer 0
      Fimescolha
   Ate opc = 0

   total := total + bebidas + lanches + acompanhamentos
   Escreval("....................................")
   Escreval("")
   Escreval("valor total R$", totaL, ",00")
   Escreval("....................................")
Fimalgoritmo