ProjetoHumQueCaro
=================

Repositório que conterá as atualizações do projeto HumQueCaro




package humQueCaro.interfaces;

import humQueCaro.beans.Cliente;
import humQueCaro.beans.Produto;
import humQueCaro.beans.Usuario;
import humQueCaro.exceptions.HumQueCaroException;

public interface FachadaBd{

	void addUsuario(Usuario usuario) throws HumQueCaroException;

	void removeUsuario (Usuario usario) throws HumQueCaroException;

	Usuario buscaUsuario (String email) throws HumQueCaroException;

	void alteraUsuario (String atributo, String novoValor) throws HumQueCaroException;

	void addProduto (Produto produto) throws HumQueCaroException;

	void removeProduto (Produto produto) throws HumQueCaroException;

	Produto buscaProduto (String codigo) throws HumQueCaroException;

	void alteraProduto (String codigo, String atributo, String novoValor) throws HumQueCaroException;

	void addCliente (Cliente cliente) throws HumQueCaroException;

	void removeCliente (Cliente cliente) throws HumQueCaroException;

	Cliente buscaCliente (String telefone) throws HumQueCaroException;

	void alteraCliente (String telefone, String atributo, String novoValor) throws HumQueCaroException;

}
