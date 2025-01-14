# LaTeX-класс `bmstu`

<a href='https://www.ctan.org/pkg/bmstu'>![Version shield](https://img.shields.io/ctan/v/bmstu)</a>
<a href='https://www.latex-project.org/lppl/'>![License shield](https://img.shields.io/ctan/l/bmstu)</a>
<a href='#'>![TestVKR build shield](https://img.shields.io/badge/TestVKR-build%20216-orange)</a>

LaTeX-класс `bmstu` призван упростить создание отчетов и расчетно-пояснительных записок студентами МГТУ им. Н. Э. Баумана. Пакет, содержащий класс, размещен в [CTAN](https://ctan.org/pkg/bmstu).

Особенности класса:
* генерация титульных страниц для всех основных типов работ — отчетов, курсовых, научно-исследовательских, дипломных;
* генерация реферата с подсчетом количества объектов;
* генерация списков определений и сокращений;
* генерация других шаблонных элементов документа;
* команды для упрощения работы с изображениями и листингами.

Сгенерированные файлы соответствуют [требованиям МГТУ им. Н. Э. Баумана](https://mf.bmstu.ru/info/uu/ot/norm_docs/docs/polozhenie_normcontrol_pril1.pdf) и [ГОСТ 7.32-2017](https://docs.cntd.ru/document/1200157208). Расчетно-пояснительные записки успешно проходят проверку программы TestVKR (сборка 216).

Примеры использования команд и окружений представлены в файлах [bmstu-examples.tex](bmstu/examples/bmstu-examples.tex) и [bmstu-examples.pdf](bmstu/examples/bmstu-examples.pdf). Приведены шаблоны для разработки [отчетов](templates/report/), [расчетно-пояснительных записок к курсовым работам](templates/coursework/), [отчетов по научно-исследовательским работам](templates/research/) и [расчетно-пояснительных записок к выпускным квалификационным работам](templates/thesis/).

## Установка

Перед установкой класса убедитесь, что установлен один из дистрибутивов LaTeX.

Например, для Ubuntu с дистрибутивом TeX Live:
```bash
git clone https://github.com/Orianti/bmstu-latex-class.git
cd bmstu-latex-class/
mkdir -p $(kpsewhich -var-value TEXMFHOME)/tex/latex/ && cp -R bmstu $_
```

## Использование

Для локальной разработки следует использовать компилятор PdfLaTeX и biber в качестве инструмента сборки библиографии. Использование bibtex вместо biber может привести к некорректному отображению ссылок.

## Вклад в разработку

Если вы обнаружили некорректное поведение команд пакета, несоответствие требованиям, опечатки или прочие недочеты, пожалуйста, создайте Issue. Там же вы можете оставить свои предложения для улучшения пакета. Также вы можете непосредственно поучаствовать в разработке, создав Pull Request.

## Лицензия

Файлы, перечисленные в [manifest.txt](bmstu/manifest.txt), распространяются по лицензии [The LaTeX Project Public License](https://www.latex-project.org/lppl/).

Файл [bmstu-logo.pdf](bmstu/bmstu-logo.pdf) является гербом МГТУ им. Н. Э. Баумана и защищен авторским правом. Распространяется по принципам свободного использования произведений (ст. 1274 ГК РФ).

---

Copyright © Новиков М. Р., 2020–2023
