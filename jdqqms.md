代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ouozrvod.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3eckmiuju.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3kxiaeezd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3rvkepizv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3mlchszth.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yxpkapeu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rmlpdxje.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3kqtnaqis.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3zjbrejyy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3lnanwfnj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3bmdzhjwu.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bvnovfst.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3gxhburvj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3atufmgjl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mnnetasq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qreiedno.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jvdrfjrf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3gvdbmsab.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3iggjtqtv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3adrywsnf.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3blqufauc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3yaaeepuo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3efqjrpzi.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3jokgllbh.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3hdnnonye.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3virmnhnl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3xocmkaiz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qlxtiwor.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3bcemmcoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qmjidbqs.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3lzjipkca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wtijaoso.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3npdrvuqk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3svozxabe.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3jwekntgi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bmfkdtyn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ryjsgrux.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lvpxceyn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3wvzgozzp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3nlmwrayd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zaxztpez.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3biflyrba.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3vqhsfkma.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsgpnotm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3digbymwf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zzufqeeh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ebihrpxc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3kvsqzdjv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3rflsuzeo.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ujcsbomh.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3kfvoxtlj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3xqurtody.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhazrqxf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmhgyxpk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3sycffupr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqlhroki.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vdeonhnb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3tpncyurd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3lranjoqu.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3kkwpdbnm.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3qyhpivcy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3itdrmrap.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3nakezaah.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3tulzmpby.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ywwglhed.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3wexicrwp.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3okidaeiu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3dceknfnx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ekcbdmux.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3wruchiys.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjvmipiq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3knmmvwfe.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3airxiufv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3fyrjfevq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3tvftrwso.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3anonzqse.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3balgfulu.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3emgfgxkz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3tqmehwqv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3bvekiwqf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3xstpaokl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3rrgquxsh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3lunwpbht.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3fokqphbu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3nseyghce.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3jfsjrumu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3rokzkvuq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ayjtxcol.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3gzvcjxas.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nmqqszdp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nudieehl.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ovpidwsf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3fhtjznbo.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3cgvcboss.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ybqdwsae.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3qjxojxyg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3wulzaevl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sgtfybej.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3glaqaqlh.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3saxtxkui.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ywdkwnav.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3oydxxfqp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3haxfoqxi.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3unwsaiuo.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ajfebdop.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3bgdzvrnk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctftlbrk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbxpfgun.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmicikok.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pyqvquhq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3tayftsss.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ipwthoyq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3oeixmayi.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3wvcnxpbr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3vunzhsih.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3zrdrghht.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xrkptexh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3zdkqdjwg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3lrhixxdt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3vlrasfnw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3cuujcldu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3licmjrpp.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3tdpxyazp.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3mvcmjqgp.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3kkwbgrnw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gackjunl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ldpouwat.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uapdsaqu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3tezhlhff.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3gzntjyzv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3jpalzbxe.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3apbnklub.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3woymsgpa.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3idnekmba.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kzkiiutq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3byaaolvb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3awoztbsk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3rylppghe.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3aquvgskn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3wofwftas.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3apkafoxj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3hdkbeyds.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3pzrfpcrl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3scqpcwkw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ooecumwl.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3fralxwbz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3dsrvnafl.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3stomutem.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3enunnwor.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3dcjokauw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3rctbjwja.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3dmjavkil.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hhsohkhc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ffksqjqp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3afvyebys.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zcnuqoby.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zmmzijfu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wwbressc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3qhcwdqbe.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3bzqqsvgr.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3sswsisyc.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yvgssqob.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gqlfaatl.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3erycmjqa.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wzcmxwty.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3unumomcu.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mqsjqvpl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3mznvvoqn.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3uqvborgw.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3eztqlobu.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3sbworzxd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3lznmsucx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3cvgmaukk.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3giojigpj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3twjitbqp.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3avrdwjai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cegxgkyc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tborznch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmvojqgw.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tgsnbcjq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3nthhplib.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qutkuxlc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fiphnrpv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgfkuzki.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3eocthxyr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wuyxpcfa.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3lcsxjolw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rnbqmtcw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3hdusibpt.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3sjmhesbf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3wgazulii.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3trienokc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3exbfnume.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3uaehrkpr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3flnpbbcq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3isvfhebz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3stobzfxj.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3plgppsnz.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3nkxhocnb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3lypafkyi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jwqscccf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3tmotxmho.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3tdamcgpi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3vxhdabrk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3mafmxmwr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ktjpuxvy.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3eiddrzxl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3knvkigtv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jgilbkcc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ffqhvuss.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3wfauoudo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3zuthzlov.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3tilbirvp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3orzqassm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lzuravyi.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3gpavqltf.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ofaheoev.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ykssprys.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3yywbvbfe.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ngvhxbsi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3dvofhlzl.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3tjpwpuzw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ovjmmmzg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ehfidhvw.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3rlgalsmy.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3zldiqzvz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3npfdhkpo.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zsqudugm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ehjacyql.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ldhdfzhl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3azshpufg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3puxkkrls.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dkpfiban.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3hauzkqsu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3wosgqxuv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3syqzjaxe.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3cvlqchyu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ugocqbjw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3pwpkajvk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3bvuvlevx.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3yilwxhrg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3dobwvhvp.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3iohqsjky.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3rtqtzdsp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3vawsuepx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlctzbzb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3acplrqla.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3zuztkmkg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3dovhxyrt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ayaawutx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gyhyohxh.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3vkxzukya.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3abzrbdry.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ckntlssk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qfcgubuy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3etnwqrwy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3pucpqcym.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3acfmefcn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vmxmifpf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dxvetcwm.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3kbttefhr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3nqoqrgoq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3sprgqtun.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tmgdnbwt.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ekcjltiy.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3afwwkjkp.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3szqykqpy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3vgletdzt.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3znhbhjsi.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3pzuadehu.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3evolspnm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ilgdbtei.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qwvufihi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3nquikwrt.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3povkeoru.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3mzyvbbnh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3npytcywf.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3jwcvcwkc.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ucqsnppg.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3omlabfml.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3wdcolnvt.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3sschfmah.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3levaeoru.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3jlzfcdlr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3xpiezjrf.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3owrkcmtm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3gujiaiup.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3daovllql.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3htdunmiu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddpmaefv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3xhgxcmio.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3riuiubuc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwqocxno.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3cnqgsezh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3preedsuc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3gdirfpqs.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3znzsqqyu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3tfzvmdyo.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wklbwsxk.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3sikpqhmv.html


<!-- 参考信息 -->