<head>
  <meta charset="utf-8">
  <title>CNIT 133 - Homework 4 Part 2</title>
  <meta name="description" content="Web Page for HW Assignment 4 of CNIT 133 - Javascript">
  <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=yes">
  <!-- Bootstrap CDN Link -->
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css" integrity="sha384-Vkoo8x4CGsO3+Hhxv8T/Q5PaXtkKtu6ug5TOeNV6gBiFeWPGFN9MuhOf23Q9Ifjh" crossorigin="anonymous">
  <!-- Custom CSS Link -->
  <link rel="stylesheet" href="css/styles.css">
</head>
<body>
 <section>
    <p class="explanation">Below, this is a table that displays compound interest on a principal of $1,000 for interest rates of 5%, 6%, and 7%, for years 1 through 10.</p>
    <div class="hw4-part1-divbox">
      <h2>Compound Interest!</h2><br>
      <script>

      for (var i = 0.05; i <= 0.07; i += 0.01){
        document.write("<table style='border: 1px solid black; width: 100%; background-color: black; color: black; table-layout: fixed; border-collapse: collapse; padding: 20px;'> <tr> <th style='border: 1px solid black; padding: 8px;'> Year </th> <th style='border: 1px solid black; padding: 8px;'> Amount On Deposit </th> <th style='border: 1px solid black; padding: 8px;'> Interest Rate </th> </tr> </table>");
          for (var j = 1; j <= 10; j++){
            var a, p, r, n, inner;
            p = 1000;
            r = i;
            n = j;
            inner = 1 + r;
            a = p * Math.pow(inner, n);
            a = a.toFixed(2);
            var currFormatter = new Intl.NumberFormat(undefined, {style: "currency", currency: "USD"});
            var fc;
            fc = currFormatter.format(a);
            document.write("<table style='width: 100%; text-align: left; table-layout: fixed;'><tr><td style='border: 1px solid black; padding: 8px;'>" + j + "</td><td style='border: 1px solid black; padding: 8px;'>" + fc + "</td><td style='border: 1px solid black; padding: 8px;'>" + i.toFixed(2) + "%</td></tr></table>");
          }
        }
<section>
    <p class="explanation">Below, a table printed via JS displays calculated, compound interest on a principal of $1,000 for interest rates of 5%, 6%, and 7%, for years 1 through 10.</p>
    <div class="hw4-part1-divbox">
      <h2>Compound Interest Demo:</h2><br>
      <script>

      for (var i = 0.05; i <= 0.07; i += 0.01){
        document.write("<table style='border: 1px solid black; width: 100%; background-color: black; color: red; table-layout: fixed; border-collapse: collapse; padding: 20px;'> <tr> <th style='border: 1px solid black; padding: 8px;'> Year </th> <th style='border: 1px solid black; padding: 8px;'> Amount On Deposit </th> <th style='border: 1px solid black; padding: 8px;'> Interest Rate </th> </tr> </table>");
          for (var j = 1; j <= 10; j++){
            var a, p, r, n, inner;
            p = 1000;
            r = i;
            n = j;
            inner = 1 + r;
            a = p * Math.pow(inner, n);
            a = a.toFixed(2);
            var currFormatter = new Intl.NumberFormat(undefined, {style: "currency", currency: "USD"});
            var fc;
            fc = currFormatter.format(a);
            document.write("<table style='width: 100%; text-align: left; table-layout: fixed;'><tr><td style='border: 1px solid black; padding: 8px;'>" + j + "</td><td style='border: 1px solid black; padding: 8px;'>" + fc + "</td><td style='border: 1px solid black; padding: 8px;'>" + i.toFixed(2) + "%</td></tr></table>");
          }
        }

      </script>
      <table style="border: 1px solid black; width: 100%; background-color: black; color: red; table-layout: fixed; border-collapse: collapse; padding: 20px;"> 
        <tbody>
          <tr> 
            <th style="border: 1px solid black; padding: 8px;"> Year </th> 
            <th style="border: 1px solid black; padding: 8px;"> Amount On Deposit </th> 
            <th style="border: 1px solid black; padding: 8px;"> Interest Rate </th> </tr> </tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">1</td><td style="border: 1px solid black; padding: 8px;">$1,050.00</td><td style="border: 1px solid black; padding: 8px;">0.05%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">2</td><td style="border: 1px solid black; padding: 8px;">$1,102.50</td><td style="border: 1px solid black; padding: 8px;">0.05%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">3</td><td style="border: 1px solid black; padding: 8px;">$1,157.63</td><td style="border: 1px solid black; padding: 8px;">0.05%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">4</td><td style="border: 1px solid black; padding: 8px;">$1,215.51</td><td style="border: 1px solid black; padding: 8px;">0.05%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">5</td><td style="border: 1px solid black; padding: 8px;">$1,276.28</td><td style="border: 1px solid black; padding: 8px;">0.05%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">6</td><td style="border: 1px solid black; padding: 8px;">$1,340.10</td><td style="border: 1px solid black; padding: 8px;">0.05%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">7</td><td style="border: 1px solid black; padding: 8px;">$1,407.10</td><td style="border: 1px solid black; padding: 8px;">0.05%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">8</td><td style="border: 1px solid black; padding: 8px;">$1,477.46</td><td style="border: 1px solid black; padding: 8px;">0.05%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">9</td><td style="border: 1px solid black; padding: 8px;">$1,551.33</td><td style="border: 1px solid black; padding: 8px;">0.05%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">10</td><td style="border: 1px solid black; padding: 8px;">$1,628.89</td><td style="border: 1px solid black; padding: 8px;">0.05%</td></tr></tbody></table><table style="border: 1px solid black; width: 100%; background-color: black; color: red; table-layout: fixed; border-collapse: collapse; padding: 20px;"> <tbody><tr> <th style="border: 1px solid black; padding: 8px;"> Year </th> <th style="border: 1px solid black; padding: 8px;"> Amount On Deposit </th> <th style="border: 1px solid black; padding: 8px;"> Interest Rate </th> </tr> </tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">1</td><td style="border: 1px solid black; padding: 8px;">$1,060.00</td><td style="border: 1px solid black; padding: 8px;">0.06%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">2</td><td style="border: 1px solid black; padding: 8px;">$1,123.60</td><td style="border: 1px solid black; padding: 8px;">0.06%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">3</td><td style="border: 1px solid black; padding: 8px;">$1,191.02</td><td style="border: 1px solid black; padding: 8px;">0.06%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">4</td><td style="border: 1px solid black; padding: 8px;">$1,262.48</td><td style="border: 1px solid black; padding: 8px;">0.06%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">5</td><td style="border: 1px solid black; padding: 8px;">$1,338.23</td><td style="border: 1px solid black; padding: 8px;">0.06%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">6</td><td style="border: 1px solid black; padding: 8px;">$1,418.52</td><td style="border: 1px solid black; padding: 8px;">0.06%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">7</td><td style="border: 1px solid black; padding: 8px;">$1,503.63</td><td style="border: 1px solid black; padding: 8px;">0.06%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">8</td><td style="border: 1px solid black; padding: 8px;">$1,593.85</td><td style="border: 1px solid black; padding: 8px;">0.06%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">9</td><td style="border: 1px solid black; padding: 8px;">$1,689.48</td><td style="border: 1px solid black; padding: 8px;">0.06%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">10</td><td style="border: 1px solid black; padding: 8px;">$1,790.85</td><td style="border: 1px solid black; padding: 8px;">0.06%</td></tr></tbody></table><table style="border: 1px solid black; width: 100%; background-color: black; color: red; table-layout: fixed; border-collapse: collapse; padding: 20px;"> <tbody><tr> <th style="border: 1px solid black; padding: 8px;"> Year </th> <th style="border: 1px solid black; padding: 8px;"> Amount On Deposit </th> <th style="border: 1px solid black; padding: 8px;"> Interest Rate </th> </tr> </tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">1</td><td style="border: 1px solid black; padding: 8px;">$1,070.00</td><td style="border: 1px solid black; padding: 8px;">0.07%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">2</td><td style="border: 1px solid black; padding: 8px;">$1,144.90</td><td style="border: 1px solid black; padding: 8px;">0.07%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">3</td><td style="border: 1px solid black; padding: 8px;">$1,225.04</td><td style="border: 1px solid black; padding: 8px;">0.07%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">4</td><td style="border: 1px solid black; padding: 8px;">$1,310.80</td><td style="border: 1px solid black; padding: 8px;">0.07%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">5</td><td style="border: 1px solid black; padding: 8px;">$1,402.55</td><td style="border: 1px solid black; padding: 8px;">0.07%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">6</td><td style="border: 1px solid black; padding: 8px;">$1,500.73</td><td style="border: 1px solid black; padding: 8px;">0.07%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">7</td><td style="border: 1px solid black; padding: 8px;">$1,605.78</td><td style="border: 1px solid black; padding: 8px;">0.07%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">8</td><td style="border: 1px solid black; padding: 8px;">$1,718.19</td><td style="border: 1px solid black; padding: 8px;">0.07%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">9</td><td style="border: 1px solid black; padding: 8px;">$1,838.46</td><td style="border: 1px solid black; padding: 8px;">0.07%</td></tr></tbody></table><table style="width: 100%; text-align: left; table-layout: fixed;"><tbody><tr><td style="border: 1px solid black; padding: 8px;">10</td><td style="border: 1px solid black; padding: 8px;">$1,967.15</td><td style="border: 1px solid black; padding: 8px;">0.07%</td></tr></tbody></table>
    </div>
        </section>        
  <!-- Bootstrap JS CDN Links -->
  <script src="https://code.jquery.com/jquery-3.4.1.slim.min.js" integrity="sha384-J6qa4849blE2+poT4WnyKhv5vZF5SrPo0iEjwBvKU7imGFAV0wwj1yYfoRSJoZ+n" crossorigin="anonymous"></script>
  <script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.0/dist/umd/popper.min.js" integrity="sha384-Q6E9RHvbIyZFJoft+2mJbHaEWldlvI9IOYy5n3zV9zzTtmI3UksdQRVvoxMfooAo" crossorigin="anonymous"></script>
  <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/js/bootstrap.min.js" integrity="sha384-wfSDF2E50Y2D1uUdj0O3uMBJnjuUD4Ih7YwaYd1iqfktj0Uod8GCExl3Og8ifwB6" crossorigin="anonymous"></script>
</body>
  <br>
      <i>~Jordan Hanks<i>
