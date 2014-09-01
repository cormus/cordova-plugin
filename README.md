# phonegap-cormus-form

Plugin documentation: [doc/index.md](doc/index.md)

```
	function listOptions(){
                
		var lista = ['alex', 'aline', 'ana', 'vitória', 'João', 'Carlos', 'Saulo', 'Pedro', 'Jessica'];
		
		navigator.notification.listOptions(
			'Seleciona um usuário:',
			lista,
			function(i)
			{
				if(i)
				{
					alert(lista[i - 1]);
				}
				else
				{
					alert('Cancelou');
				}
			},
			'Cancelar'
		);
	}

	function checklist(){
		
		var lista = ['alex', 'aline', 'ana', 'vitória', 'João', 'Carlos', 'Saulo', 'Pedro', 'Jessica'];
		
		navigator.notification.checklist(
			'Seleciona um usuário:',
			lista,
			function(i)
			{
				if(i)
				{
					alert(i);
				}
				else
				{
					alert('Cancelou');
				}
			},
			[1],
			'Cancelar'
		);
	}
```