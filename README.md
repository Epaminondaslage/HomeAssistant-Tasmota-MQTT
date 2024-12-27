<td style="width: 20%;"><img src="imagens/top_ha_tasmota_mqtt.png" width="100%"></td>


# Integração com o Home Assistant

Para integrar o Tasmota com o Home assistant, siga os passos mostrados abaixo. Caso prefira acompanhar um video, o video [Home Assistant Tasmota Integration (HOW-TO)](https://www.youtube.com/watch?v=ownHLQbAZ8Y) possui um passo a passo de como realizar a integração.

Para configurar a descoberta nativa do Tasmota no Home Assistant, abra o console e envie o comando **SetOption19 0**

![Alt text](imagens/21.png)

Além disso, o comando **SetOption30 0** configura o icone como sendo um **switch**. Caso queira um icone de **light**, use **SetOption30 1**.

![Alt text](imagens/22.png)

Feito isso, o Home Assitant ja deve ter descoberto a nova integração automaticamente. Caso isso não ocorreu, adicione-a clicando em **+ ADICIONAR INTEGRAÇÃO**. Em seguida, clique em configurar. Caso os passos anteriores tenham sido efetuados corretamente, o tasmota sera descoberto automaticamente a adicionado como um novo dispositivo.

![Alt text](imagens/23.png)

![Alt text](imagens/24.png)

Clicar no dispositivo abre a janela de informações dele, onde podemos ver todas as entidades cadastradas. Podemos observar que o **switch** de controle do relé e o **sensor** de efeito hall foram automaticamente adicionados e ja podem ser utilizados normalmente no Dashboard.

![Alt text](imagens/25.png)

![Alt text](imagens/26.png)

![Alt text](imagens/27.png)

Finalmente, podemos ver que, além do **switch** e do **sensor**, diversas outras entidades são adicionadas automaticamente. Contudo, nem todas são habilitadas por padrão.

![Alt text](imagens/28.png)

Para abilitar uma entidade desabilitada, abra a janela de informações do dispositivo e clique na entidade que deseja habilitar.

![Alt text](imagens/29.png)

Em seguida, mude o estado do campo **Habilitado**.

![Alt text](imagens/30.png)

![Alt text](imagens/31.png)

A entidade passara a estar disponivel para ser utilizada.

![Alt text](imagens/32.png)

# Sites relacionados ao Home Assistant - Tasmota

- Site oficial do Tasmota: https://tasmota.github.io/docs/
- Documentação oficial da integração do Tasmota com Home assistant: https://www.home-assistant.io/integrations/tasmota/
- Site do MQTT Explorer: http://mqtt-explorer.com/

# Status do Projeto

![Badge em Desenvolvimento](http://img.shields.io/static/v1?label=STATUS&message=EM%20DESENVOLVIMENTO&color=GREEN&style=for-the-badge)
