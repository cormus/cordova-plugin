# phonegap-cormus-form

Plugin documentation: [doc/index.md](doc/index.md)

```
		function clickAlert(){
					
			var lista = ['alex', 'aline', 'ana', 'vit�ria', 'Jo�o', 'Carlos', 'Saulo', 'Pedro', 'Jessica'];
					
			navigator.notification.alex(
				'Selecione um usu�rio!',
				lista,
				function(i)
				{
					alert(lista[i - 1]);
				}
			);
		}
```