# phonegap-cormus-form

Plugin documentation: [doc/index.md](doc/index.md)

```
	function listOptions(){
                
		var lista = ['alex', 'aline', 'ana', 'vit�ria', 'Jo�o', 'Carlos', 'Saulo', 'Pedro', 'Jessica'];
		
		navigator.notification.listOptions(
			'Seleciona um usu�rio:',
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
		
		var lista = ['alex', 'aline', 'ana', 'vit�ria', 'Jo�o', 'Carlos', 'Saulo', 'Pedro', 'Jessica'];
		
		navigator.notification.checklist(
			'Seleciona um usu�rio:',
			lista,
			function(data)
			{
				if(data)
				{
					var array = JSON.parse(data);
					array.forEach(function(value, index) {
						if(value)
						{
							alert(lista[index]);
						}
					});
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