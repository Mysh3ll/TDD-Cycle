**Le cycle TDD : Les 3 lois du TDD**

[Reference: UncleBob](http://butunclebob.com/ArticleS.UncleBob.TheThreeRulesOfTdd)

Jusqu'à présent, dans ce cours, nous avons couvert une partie de la théorie sur les tests unitaires et je vous ai donné les bases des tests unitaires, la structure d'un test, etc. Nous allons maintenant aborder la théorie concernant spécifiquement le **TDD**.

La première chose que j'aimerais aborder, ce sont **les trois lois du TDD**. Il s'agit d'une sorte de formulation de la pratique du **TDD** telle qu'elle a été créée par _Robert C. Martin_. Vous pouvez la trouver sur son site web.

* La première loi, ou règle, est que vous n'êtes pas autorisé à écrire du code de production à moins que ce ne soit pour faire... un test unitaire 
défaillant, c'est-à-dire qu'à moins d'avoir un test unitaire défaillant, vous ne pouvez pas écrire de code de production et tout code de production que vous écrivez ne doit servir qu'à faire passer ce test unitaire.

* La seconde est que vous n'avez pas le droit d'écrire plus d'un test unitaire qu'il n'en faut pour qu'il échoue. Les échecs de compilation sont des échecs.

* La troisième est que vous n'avez pas le droit d'écrire plus de code de production qu'il n'en faut pour faire passer ce seul test unitaire défaillant. Ce qui est similaire à la première, mais dit plus spécifiquement que vous ne pouvez avoir qu'un seul test défaillant à un moment donné et que votre but est de faire passer ce seul test. Une fois que ce test est passé, vous devez écrire un test unitaire aussi petit que possible pour qu'il échoue avant d'écrire un tout petit bout de code de production pour faire passer ce test unitaire.

Ce sont des lois ou des règles qui régissent la micro-mécanique du **TDD**. Les suivre vous oblige à prendre de très petites mesures systématiques. Nous verrons exactement à quoi ressemble l'application de ces règles dans le Guide de démarrage, dans cette section, pour cet exercice.

Notez également qu'il s'agit de règles intentionnellement très didactiques, de règles fixes en quelque sorte. Nous sommes en train d'apprendre une nouvelle compétence, et le fait de suivre ce type de règles peut nous aider, plutôt que d'improviser. Je vous encourage à les suivre le plus fidèlement possible pour commencer. Elles peuvent sembler onéreuses, elles peuvent sembler un peu dures, et une fois que vous serez plus avancés dans votre voyage dans le **TDD**, vous pourrez peut-être commencer à les assouplir.

Et nous parlerons à un moment donné de la façon d'assouplir les règles du **TDD** pour aller plus vite. Mais cela couvre à peu près ces trois lois.
Nous les appliquerons dans le prochain exercice.