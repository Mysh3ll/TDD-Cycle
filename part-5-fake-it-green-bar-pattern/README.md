🔄🟢🔴 **Le cycle TDD : Le fake it green bar pattern**

Le dernier élément théorique de cette section avant d'aborder le **Kata pierre, papier, ciseaux** est le **_fake it green bar pattern_**. Avant de nous plonger dans le fake it green bar pattern, expliquons ce qu'est un pattern.

Les patterns sont simplement des façons connues de résoudre des problèmes courants. Vous êtes peut-être déjà familier avec les patterns sous la forme de design patterns tels que le pattern Factory ou le pattern Repository. Ce sont des modèles qui aident à résoudre des problèmes couramment rencontrés dans le code.

Le fake it green bar pattern aide à résoudre le problème de passer rapidement d'un test rouge qui échoue à un test vert qui réussit. Il existe des moyens connus pour passer au vert. [Kent Beck](https://www.kentbeck.com/) a introduit l'idée de fake it green bar pattern dans son livre _"Test Driven Development by Example"_.

Vous vous demandez peut-être pourquoi ces patterns sont nécessaires. Eh bien, l'une des principales choses que vous essayez de faire dans le cadre du **TDD** est de franchir les étapes du cycle de **red-green-refactor** très rapidement. C'est une façon de travailler assez différente, cela semble différent, mais c'est ce qui donne au **TDD** son caractère unique dans son approche : le retour d'information extrêmement rapide que vous obtenez.

Et des choses étranges se produisent lorsque vous faites cela. Vous constatez que le code dont vous avez besoin est beaucoup plus petit que celui dont vous pensiez avoir besoin. Nous essayons donc de nous discipliner pour écrire juste assez de code. Souvenez-vous de l'une des trois lois : _juste assez de code pour que le test passe_.

Voyons cela plus concrètement avec un exemple. Supposons que nous ayons le test suivant : 🔄🟢🔴

```ts
it("should return 'Hello Mysh3ll'", () => {
    const actual = hello("Mysh3ll");
});
```

Dans cet exemple, nous avons un test qui appelle une fonction hello avec le nom "Mysh3ll" et s'attend à ce que le résultat soit "Hello Mysh3ll". Pour l'instant, nous n'avons pas implémenté la fonction hello, donc le test échouera. Nous sommes dans l'état **rouge du TDD**.

Pour passer au vert, nous allons effectuer une _fausse implémentation_. Nous allons créer une fonction vide pour hello : 🔄🟢🔴

```ts
function hello(name: string) {
    // Fausse implémentation
}
```

Maintenant, si nous exécutons à nouveau le test, il passera car la fonction existe. Nous sommes donc passés à l'état **vert du TDD**.

À ce stade, nous pouvons ajouter notre attente dans le test : 🔄🟢🔴

```ts
it("should return 'Hello Mysh3ll'", () => {
    const actual = hello("Mysh3ll");
    expect(actual).toBe("Hello Mysh3ll");
});
```

Maintenant, si nous exécutons le test à nouveau, il échouera car notre implémentation actuelle ne renvoie pas la bonne valeur. Nous sommes donc de nouveau dans l'état **rouge du TDD**.

Maintenant, nous pouvons utiliser le fake it green bar pattern pour faire passer le test rapidement. Au lieu d'écrire un algorithme complet pour générer le bon résultat, nous allons simplement retourner la chaîne "Hello Mysh3ll" directement dans notre fonction hello : 🔄🟢🔴

```ts
function hello(name: string): string {
    return "Hello Mysh3ll"; // Fausse implémentation
}
```

Maintenant, si nous exécutons le test, il passera car notre fausse implémentation renvoie la valeur attendue. Nous sommes de nouveau dans l'état **vert du TDD**.

À ce stade, nous pouvons réfléchir à l'implémentation réelle de la fonction hello. La fausse implémentation est simplement un tremplin vers la véritable implémentation. Nous ne prévoyons pas de laisser cette version finale telle quelle. Au lieu de cela, nous utiliserons un autre test pour guider une véritable implémentation.

En pratique, nous commençons souvent par renvoyer des valeurs littérales comme nous l'avons fait ici, puis nous introduisons des instructions conditionnelles ou des boucles au fur et à mesure que le besoin se fait sentir, jusqu'à ce que nous ayons une fonction complète.

Le fake it green bar pattern est très utile lorsque vous abordez un problème nouveau ou si vous n'êtes pas sûr de l'algorithme à utiliser et que vous voulez créer un contexte pour commencer à identifier des modèles émergents.

Nous aborderons d'autres patterns dans des exercices ultérieurs, mais pour le **Kata pierre, papier, ciseaux** que nous allons réaliser, ce pattern devrait être suffisant. Passons donc à la phase de mise en route où nous appliquerons ces concepts de manière plus concrète.

Allez, c'est parti ! 🔄🟢🔴