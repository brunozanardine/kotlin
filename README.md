class Usuario(
  val Nome : String,
   val Idade : String,
   val cpf : String, ) {

  init{
    println("Usuario")
  }

  fun
    printarObjeto() {
    println("Nome: $Nome")
    println("Idade: $Idade")
    println("cpf: $cpf")
    println()
  }
}



class Livro(
  val Nome : String,
  val Tema : String,
  val Autor : String,
  val Paginas: String,
  val IdLivro : String,
  val Cliente : String,
  val LivroReservado: Boolean) {

    init{
        println("Livros Emprestados")
    }

  fun
    printarObjeto() {
    println("Nome: $Nome")
    println("Tema: $Tema")
    println("Autor: $Autor")
    println("Paginas: $Paginas")
    println("IdLivro: $IdLivro")
    println("Cliente: $Cliente")
    println()
  }
}

class Biblioteca(
  val Nome: String,
  val Bibliotecario: String,
  val Horario: String,
  val Local: String) {

  init{
    println("Biblioteca")
  }

  fun
  printarObjeto() {
    println("Nome: $Nome")
    println("Bibliotecario: $Bibliotecario")
    println("Horario: $Horario")
    println("Local: $Local")
    println()
  }
}

fun main() {

    val biblioteca1 = Biblioteca("Biblioteca Bagual", "Bernabei", " 08:00 - 17:00", "Juveve")
    biblioteca1.printarObjeto()
    val livro1 = Livro("Sacidointer", "Internacional", "Rafael Sobis", "75", "1909","Bruno", false)
    livro1.printarObjeto()
    val livro2 = Livro("Artilheiro", "Esporte", "Roger Machado", "70", "2006","Borre", true)
    livro2.printarObjeto()
    val usuario1 = Usuario("Bruno", "18", "14523356788")
    usuario1.printarObjeto()
    val usuario2 = Usuario("Borre", "33", "86759034566")
    usuario2.printarObjeto()
    println()
}
