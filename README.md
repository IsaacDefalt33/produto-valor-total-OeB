<?php

class produto{
    private string $descricao;
    private string $unidadeMedida;
    private int $quantidade;
    private float $valorUnitario;

    public function __construct(string $descricao, string $unidadeMedida, int $quantidade, float $valorUnitario){
        $this -> descricao = $descricao;
        $this -> unidadeMedida = $unidadeMedida;
        $this -> quantidade = $quantidade;
        $this -> valorUnitario = $valorUnitario;
    }
    

   
    public function getDescricao(): string
    {
        return $this->descricao;
    }

  
    public function setDescricao(string $descricao): self
    {
        $this->descricao = $descricao;

        return $this;
    }

   
    public function getUnidadeMedida(): string
    {
        return $this->unidadeMedida;
    }

   
    public function setUnidadeMedida(string $unidadeMedida): self
    {
        $this->unidadeMedida = $unidadeMedida;

        return $this;
    }

    
    public function getQuantidade(): int
    {
        return $this->quantidade;
    }

   
    public function setQuantidade(int $quantidade): self
    {
        $this->quantidade = $quantidade;

        return $this;
    }

    
    public function getValorUnitario(): float
    {
        return $this->valorUnitario;
    }

   
    public function setValorUnitario(float $valorUnitario): self
    {
        $this->valorUnitario = $valorUnitario;

        return $this;
    }
}


for ($i = 0; $i < 3; $i++){
    $descricao = readline( "Digite a descrição do produto: ");
    $quantidade = readline( "digite a quantidade do produto: ");
    $valorUnitario = readline( "digite o valor unitário do produto:");
    $unidadeMedida = readline( "digite a unidade de medida do produto: ");
    switch($i){
        case 0:
            $produto1 = new produto($descricao , $quantidade, $valorUnitario, $unidadeMedida);
            break;
            case 1:
                $produto2 = new produto($descricao , $quantidade, $valorUnitario, $unidadeMedida);
                break;
                case 2:
                    $produto3 = new produto($descricao , $quantidade, $valorUnitario, $unidadeMedida);
    }
    
}
 
