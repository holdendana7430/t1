代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3slhcborn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3kaqlbzvj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3gjkvqlgq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3gzytajle.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3bvnympqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rvasxrqb.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3wjpkkrhs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jnnhnewt.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3vxmpupsy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3tmhffpvy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwtvmoht.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3demnhttd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bbohnacj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vcjmwpqr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3hzkrulrt.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3cldrfbqm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nclfagpw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3zlqjtngk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3rssznbtk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3ryzbxcgp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zorveqia.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3spibxaty.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hdkniaoo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3bpkwtbdu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ulggmbtr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3afnakuuv.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ieqqzcal.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3wejotlmm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oerjnhij.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3exrxgmet.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zuuhfwns.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3foggskyd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3doikhyxj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3vcmwykgd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3krzpxegj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3movbftqz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nfzhlrca.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmtcpjnf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3xwwjfvfp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wzmpzmhl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3gwkgplpq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3kebhvpen.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3kvqjjhtx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3boveddxy.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dixmsgzc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3kdqhtpli.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzokgiqr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yvxmfkoy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xankgaas.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mddfuxju.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ewxzzocn.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3uwahrrsf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3rupblbgd.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ebazediu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3wntahwrh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kixabtow.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zxwdznnp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3uwdupyam.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ccfwwkyx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3vuatvsmd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qydijaok.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3etbbwcqh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3zusscofl.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3meecnjfs.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckbiiieu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cpwisxxf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjrkppjj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3totwadgd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3tjgqfwvu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3wvboupha.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pxlbjbmd.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ckcfwnwg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3xrgnijfv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wywjfgtt.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3evtlfqeh.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ydepvqgf.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hplpiwst.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wrqxzltz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3qqwxzseb.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3iyhugvet.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3xlztknsa.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3tfevwskb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3eryxdwjt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jntbqlzj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjmymoyo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3swodhqcz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xmqjxnaj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3hxzadywx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mehunzwr.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3wnshwhne.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3nxvkgpgo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tammjasf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3hcneqgbr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3qdhqoatq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3odgbjdkj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3dokrljjs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3smcbiuzb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3wtaoahoz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3magfgrov.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3xulsrsih.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3fxktjuqg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gsgxyxex.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3sekbpixc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cjawtyle.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ieifvuck.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ftnfwxpx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3uqraqvye.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3qgvzypeq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3wcmwxlap.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3klfxoxlq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3aysvoqeg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jroelxbr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3yguhfaze.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3tyeugiqq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3dbiptdbm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3rekpckkg.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3lpurzikz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3bhgjrozh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3dqdfvoqc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nwniznwz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3yefgwkma.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3fmwmznes.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3bologexl.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3gjuuwrcd.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3poprfzrw.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3twmjpzgb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3gprvycfh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ihhletzo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nfdabxst.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tveujorl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wxqivzzi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3xqgiksgz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3iuzcqfbv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kysgsful.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3tlzvyqds.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3jejaeokf.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3rnioewsl.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3luwntdgo.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ogkiwhzu.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kogknuvw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pgihdsmp.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uwopxojm.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3swoonguo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3lqjkzmzl.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3wasgoxli.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3houttmdt.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vlyuysii.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3tqpwrckf.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3kkxqceck.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nedknvdl.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3codhemhu.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3hirjrbae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uwavjidb.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iqcklcxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ybjcrsoj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3rxfvvrgy.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3fjhsqbji.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3thhhrurd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxzmrybk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xrwxyfkp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bypitczd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3tjhuwmxc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3owxumdla.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfshbino.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3wjiitadc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3pqkslplu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uodgjdus.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3brgzuisp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3whnsdmvr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3dmsbzfyk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3trsrzdom.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3dihiexat.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ilkrctgl.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3njdrbomk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3hdhwxrmk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3xrdnjlxz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3irmngfti.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3dhymyvfh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3lzlhwsgb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3okkdgwml.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3bmkzwnem.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3fhslxbkb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3iamobdna.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3epmeujjn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3jytznakt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hjcbrprs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3jskjqusr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3copsxwtb.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3pjwvzuyr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bgfxbcak.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3atjjmxez.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3rlrjjaas.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3logliaxw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3czzduoos.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3uyjrngio.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3zdzskipt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3bzxtckng.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3sxokhwuo.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3tcrfjdgv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3isxomjix.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3sgqpemgj.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ubmqcikk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3tspclksj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ajxcsdif.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3pgtezywd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3dajilrsr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3csphnewn.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ogljtppk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ydpeaxby.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3hjpmhkba.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3pzzegdsm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3fgnuxiko.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3jbjdqrlo.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3wmcpvpth.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3kkehrlda.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3pesqkhsy.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ryxvpdma.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3jswwmqin.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jcxuohse.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3bfgjuaxa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxfmbdan.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ognzjowa.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qpwtuhpp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3mifdnkwn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3tybooniw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3lkzqcyge.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fipogdfn.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3lryvxtcl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vlgrgcaf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3eqdpjsdp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3niwokchc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3aorohbko.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqwbjpre.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3rajrylpn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3kazonmow.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gmzzmwmd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3cxeckqmo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3fuzmwchl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3fgjitrfw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ktvaytgr.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ivyvahlc.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ivqrqjus.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gvmbdtwo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3hacqzyhj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bgsbonid.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3odfksbmn.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3wgofiovv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3xowfgplt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3kbyodpow.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3drctnwlc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3gfybyptj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3elqzqgli.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3rkbfyhth.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ddyklfel.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3xblanmpx.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3nawxdrhw.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3bciaffet.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3edtgswrc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3lblzlghk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3nfxpunuc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3sqrjirlk.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3hhacaont.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dddvwwst.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3vfnaekco.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ovlzumpg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nngadmvy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3roniqkik.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyfltufz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3oubnxwqz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3trmpduhd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3snhvolul.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3mhlqsflt.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3bvlhtqah.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3gtmjbamm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ruyrluqu.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3yxvsfipp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwqdneyi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tpgwegff.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ziutjwcq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3pmbdggwa.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3vkmihdvy.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3bhbrddoi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3teyxymza.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hhzckdml.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3aynudtgf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3stwypwjc.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3tirgcipb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hfpkkvxr.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3nfhliswz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3fimmthmt.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3lklplafa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3bjqujvah.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3pcqbzswq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3uideahbs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3iwylxtci.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ulcimxrt.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3gzlaprre.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3dytujnjt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3mrnxutzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bzvjjrdh.html


<!-- 参考信息 -->