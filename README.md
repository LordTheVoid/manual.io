<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>Java программирование</title>
      <link rel="stylesheet" href="projekt.css">
      <style media="screen">
        header {
          text-align: center;
          font-size: 25px;
        }
        .import{
          position: relative;
          display: inline-block;
          cursor: pointer;
        }
        .import-up{
          visibility: hidden;
          opacity: 0;
          position: absolute;
          bottom: 120%;
          left: 0;
          /* transform: translateX(-50%); */
          background-color: red;
          color: white;
          padding: 8px 12px;
          border-radius: 6px;
          font-size: 14px;
          white-space: nowrap;
          transition: opacity 0.25s ease, visibility 0.25s ease;
          z-index: 100;
          pointer-events: none;
          box-shadow: 0 4px 12px rgba(0,0,0,0.2);
        }
        .import:hover .import-up{
          visibility: visible;
          opacity: 1;
        }
      </style>
  </head>
  <body>
    <header>
      <a href="#main_dates" class="light_blue">Основные даты в истории Java</a><br>
      <a href="#analysis" class="light_blue">Разбор Java кода</a>
    </header>
    <h1 class="white history">История Java программирования</h1>
    <p>Проект Java <b>зародился в 1991 году</b> в недрах компании <b>Sun Microsystems</b>. Трое инженеров — Джеймс Гослинг, Майк Шеридан и Патрик Ноттон — стремились создать язык, работающий на небольших электронных устройствах.</p>
    <p>Первоначально новый язык получил название <b><i>Oak</i></b>, что в переводе означает <i>«дуб»</i>. Название было предложено Джеймсом Гослингом — он вдохновился дубом, росшим под окнами его офиса. Однако в процессе подготовки к официальному выпуску выяснилось, что торговая марка с таким названием уже зарегистрирована компанией Oak Technologies.</p>
    <p>В итоге язык был переименован в Java — это слово отсылает к сорту кофе с острова <b>Ява</b> в <b>Индонезии</b>.</p>


    <h2 id="main_dates" class="white">Основные даты в создании</h2>
    <p><a target="_blank" href="Age_1991.html"><b>1991  Год</b> - Начало разработки языка Java</p></a>
    <p><a target="_blank" href="Age_1992.html"><b>1992 - 1995 Года</b> - Разработка и официальный выпуск</p></a>
    <p><a target="_blank" href="Age_1996.html"><b>1996 - 2000 Года</b> - Первое существенное изменение и набор популярности</p></a>
    <p><a target="_blank" href="Age_2001.html"><b>2001 - 2009 Года</b> - Смена эпох и трудности</p></a>
    <p><a target="_blank "href="Age_2010.html"><b>2010 - Н. В.</b> - Oracle и новые горизонты</p></a>

    <h1 class="white">Разбор кода на Java на примере кода Калькулятора</h1>
    <pre id="analysis">
      <span class="import">
<span class="orange">import</span> java.util.Scanner;
<span class="import-up">что-то явно написано, мне шепотом говорит Богдан.</span>
</span>
  <span class="orange">public class</span> Main {
      <span class="orange">public static void</span> main(String[] args) {
          Scanner scanner = <span class="orange">new</span> Scanner(System.in);

          double itog = <span class="light_blue">0</span>;

          <span class="orange">while</span> {
              System.out.print(<span class="green">"Введите первое число: "</span>);
              <span class="orange">double</span> num1 = scanner.nextDouble();

              System.out.print(<span class="green">"Введите 1 если ваше действие сложение"</span>);
              System.out.print(<span class="green">""</span>);
              System.out.print(<span class="green">"Введите 2 если ваше действие вычитание"</span>);
              System.out.print(<span class="green">""</span>);
              System.out.print(<span class="green">"Введите 3 если ваше действие умножение"</span>);
              System.out.print(<span class="green">""</span>);
              System.out.print(<span class="green">"Введите 4 если ваше действие деление"</span>);
              int action = sc.nextInt();

              System.out.print(<span class="green">"Введите второе число: "</span>);
              <span class="orange">double</span> num2 = scanner.nextDouble();

              <span class="orange">if</span>(action == <span class="light_blue">1</span>){
                itog = num1 + num2;
              }

              <span class="orange">if</span>(action == <span class="light_blue">2</span>){
                itog = num1 - num2;
              }

              <span class="orange">if</span>(action == <span class="light_blue">3</span>){
                itog = num1 * num2;
              }

              <span class="orange">if</span>(action == <span class="light_blue">4</span> & num1 != <span class="light_blue">0</span> & num2 != <span class="light_blue">0</span>){
                itog = num1 / num2;
              }

              <span class="orange">else</span>{
              System.out.print(<span class="green">"Одна из переменных равна нулю, на ноль делить нельзя!"</span>);
              }

              System.out.printf(<span class="green">"Результат:"</span> + num1, operator, num2, result);
          }
      }
  }
          </pre>
    <script src="projekt.js" type="text/javascript"></script>
  </body>
</html>
