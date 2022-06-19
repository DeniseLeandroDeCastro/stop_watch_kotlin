# StopWatch em Kotlin

<p>
O app StopWatch tem apenas uma activity. 
Seu layout contém uma exibição de texto para mostrar o tempo percorrido, 
um botão para iniciar o cronômetro,um botão que para o cronômetro, e um outro botão que faz reset.
</p>

<div align="middle">
  <h4>StopWatch</h4> 
  <img src="https://user-images.githubusercontent.com/29150094/174459973-49a7cff0-eb2c-46d1-8116-f182de010616.png" width="360" height="650" />  
</div>
<div>
<div align="middle">
<h2>O ciclo de vida de uma Activity</h2> 
</div>
  
<p>
Quando o Android cria e destrói uma Activity, ela passa pelos estados de ativada, em execução e destruída. O estado principal de uma activity é em execução ou ativada. Uma activity está em execução, quando está no primeiro plano da tela, em foco e o usuário pode interagir com ela. A activity passa a maior parte da sua vida nesse estado. Uma activity começa a ser executada depois de ser ativada e, no fim da sua vida, é destruída.
</p>
  
  <div align="middle">
  <img src="https://user-images.githubusercontent.com/29150094/174481329-71a09bf2-7ec3-444b-af18-a4ed7236781d.png" width="600" height="480" />  
  </div> </br>
  
<p>
Ao passar de ativada para destruída, a activity aciona métodos importantes do ciclo de vida: o onCreate( ) e o onDestroy( ). Esses métodos são herdados pela activity e podem ser substituídos. O método onCreate( ), é chamado logo depois da ativação da activity. Ele permite que você configure a activity e, por exemplo, chame o setContentView( ), informando ao Android qual o layout que a activity deve usar. O método onDestroy( ) é o último a ser chamado antes da destruição da activity. Uma activity pode ser destruída em diversas situações. Por exemplo, para ser finalizada, para ser recriada devido a uma mudança na configuração do dispositivo ou caso o Android tenha decidido destruí-la para liberar espaço.
</p>
</div>
<div align="middle">
<h2>O ciclo de vida: da criação à destruição</h2> 
<img src="https://user-images.githubusercontent.com/29150094/174484709-9fbb552e-eda3-4d8b-a496-203383ba57fd.png" width="250" height="480" /> 
</div>
<div>
<p>
  <ol>
    <li>A activity é ativada. O objeto activity é criado e seu construtor é executado.</li>
    <li>O método onCreate( ) é executado logo depois da ativação da activity. O código de iinicialização deve estar no método onCreate( ), pois esse método   sempre é chamado depois da ativação da activity e antes da sua execução.</li>
    <li>Uma activity está em execução quando é visível no primeiro plano e o usuário pode interagir com ela. A activity passa a maior parte da vida nesse estado.</li>
    <li>O método onDestroy( ) é executado logo depois da destruição da activity. Ele permite a realização de ações de limpeza final, como a liberação de recursos.</li>
    <li>Depois da execução do método onDestroy( ), a activity é destruída e deixa de existir.</li>
  </ol>
</p>
</div>
