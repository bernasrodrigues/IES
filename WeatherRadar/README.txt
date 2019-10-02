O ciclo de desenvolvimento de um projeto maven é composto
por varias fases sendos estas:
	-validate
	-compile
	-test
	-package
	-verify
	-install
	-deploy

Cada uma representa um estagio diferente na criação de software
As fases são obrigatoriamente executadas sequencialmente não podendo
ser nenhuma fase ser ignorada
	ex: Para executar a fase "test" teriamos que primeiro passar pela
	fase "validade" e depois pela "compile" e só depois destas serem 
	bem sucedidas, poderiamos chegar à fase "test"

Cada fase é composta por varios goals,um goal é uma tarefa especifica,
normalmente definida pelos  plugins, que contribuem para a criação e 
gestão do projeto, uma fase está completa quando são executados todos
os seus goals. Um goal pode estar atribuido a zero ou mais fases.