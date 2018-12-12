# biblioteca_logica

Projeto de Lógica 18.2


## Uso
Para usar o Projeto, você precisa baixar o NuSMV na sua versão compilada por esse [link](http://nusmv.fbk.eu/NuSMV/download/getting_bin-v2.html). Após baixar, dentro da pasta do `NuSMV/bin` terá um arquivo com nome `NuSMV`, transfira ele para a pasta do repositório, você o usará para rodar esse projeto.

### Para testar
Com o arquivo `NuSMV` na mesma pasta, use:

```sh
./NuSMV biblioteca.smv
```

### Entrar no console 

```sh
./NuSMV -int
```

### Simular

Primeiro iremos preparar o modelo, dentro do console, use:
```sh
reset
read_model -i biblioteca.smv
flatten_hierarchy 
encode_variables
build_model
```

#### Rodar estado randomicamenta:

1. Escolher o estado inicial

`pick_state -v -i`

2. Simulate ~ainda nao entendi como funciona pra gnt testar como o prof testa~
`simulate -v -i -k 0`