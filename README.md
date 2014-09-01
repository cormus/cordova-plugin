# phonegap-cormus-form

Plugin documentation: [doc/index.md](doc/index.md)

```
		function clickAlert(){
					
			var lista = ['alex', 'aline', 'ana', 'vitória', 'João', 'Carlos', 'Saulo', 'Pedro', 'Jessica'];
					
			navigator.notification.alex(
				'Selecione um usuário!',
				lista,
				function(i)
				{
					alert(lista[i - 1]);
				}
			);
		}
		
		 function checklist(){
			
			var lista = ['alex', 'aline', 'ana', 'vitória', 'João', 'Carlos', 'Saulo', 'Pedro', 'Jessica'];
			
			navigator.notification.checklist(
				'Seleciona um usuário:',
				lista,
				function(i)
				{
					alert(i);
				},
				[1]
			);
		}
```