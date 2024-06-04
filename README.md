# 02Mobile
```
O código que você apareceu é um layout XML para um aplicativo Android. Ele define uma interface de usuário usando um RelativeLayoutque contém três campos de entrada de texto ( EditText) e um botão ( Button). Aqui está a estrutura e a função de cada parte do código:

Esquema relativo :

O elemento raiz é um RelativeLayout, que permite posicionar elementos de forma relativa uns aos outros.
A largura ( android:layout_width) e a altura ( android:layout_height) RelativeLayoutsão definidas como "match_parent", o que significa que ele ocupará todo o espaço disponível do pai.
Editar Texto Título :

Um campo de entrada de texto ( EditText) com o ID editTextTitulo.
Largura ajustada para ocupar todo o espaço disponível horizontalmente ( match_parent).
Altura ajustada para ajustar ao conteúdo ( wrap_content).
Um texto de sugestão ("hint") que diz "Título".
EditText Autor :

Outro campo de entrada de texto ( EditText) com o ID editTextAutor.
Largura ajustada para ocupar todo o espaço disponível horizontalmente ( match_parent).
Altura ajustada para ajustar ao conteúdo ( wrap_content).
Posicionado abaixo do campo de título ( android:layout_below="@id/editTextTitulo").
Um texto de sugestão ("hint") que diz "Autor".
Editora EditText :

Mais um campo de entrada de texto ( EditText) com o ID editTextEditora.
Largura ajustada para ocupar todo o espaço disponível horizontalmente ( match_parent).
Altura ajustada para ajustar ao conteúdo ( wrap_content).
Posicionado abaixo do campo de autor ( android:layout_below="@id/editTextAutor").
Um texto de sugestão ("hint") que diz "Editora".
Botão Salvar :

Um botão ( Button) com o ID buttonSalvar.
Largura ajustada para ajustar ao conteúdo ( wrap_content).
Altura ajustada para ajustar ao conteúdo ( wrap_content).
Posicionado abaixo do campo da editora ( android:layout_below="@id/editTextEditora").
Texto do botão configurado como "Salvar".
Função Geral
Este layout cria um formulário simples com três campos de entrada para o usuário digitar o título, o autor e a editora de um livro, e um botão para salvar essas informações. Quando integrados em um aplicativo Android, esses campos podem ser usados ​​para coletar informações do usuário e o botão pode ser configurado para executar uma ação, como salvar os dados inseridos em um banco de dados ou enviá-los para um servidor.
```
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent">
    <EditText
        android:id="@+id/editTextTitulo"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:hint="Título" />
    <EditText
        android:id="@+id/editTextAutor"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_below="@id/editTextTitulo"
        android:hint="Autor" />
    <EditText
        android:id="@+id/editTextEditora"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_below="@id/editTextAutor"
        android:hint="Editora" />
    <Button
        android:id="@+id/buttonSalvar"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_below="@id/editTextEditora"
        android:text="Salvar" />
</RelativeLayout>
