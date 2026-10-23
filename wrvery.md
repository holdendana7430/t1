代发 wailian999

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3wikaucgi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3wrwjcwct.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3zsjklxez.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3rbtiljwe.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3okgkxdrq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3zlchyqhi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3nnxzsajo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3acdcwqrl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3jbrygxuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lzpozpde.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3xpvicoik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gpqvnsdz.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3scwtkrts.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3sshaxsht.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3kohfiduu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3leuzmeaa.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nymamkif.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vwwkmunt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3mvqcrwfb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ftqvxwyd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jnrfxlpb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3pbqsizqx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ngvvdmxz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3ejcywekh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dkgshall.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gbgqjkdc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nbtsgpvg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3qiilznea.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ekzpanho.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3btqdmpwj.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3gmuwjwid.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3hrwvdnsw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3sezygtot.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lchsicnl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjimuuci.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbdqhfdj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3mugvmsnz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3gfsylzbf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3awrucqta.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3nvouepms.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ahmivtoo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmudkadn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3apozdawg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vsaxxzao.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3jgbxsvlf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3vcqkmvql.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3yppwnfmx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ljregxjj.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3sitquixm.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3nbvwmhhr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ldsvnsnv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cprzwlqa.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jefrluwn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hhsvsbst.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3dayssefc.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3bpsdwepr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3hcvwfzdq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3mmdqyktv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3drgcmdnp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oakcazeg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3sucejyss.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3peqkdyds.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3pkzszfzt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3vpslemke.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3fhjzlmmm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3zcmccnfq.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3vefdvebg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3rnbgdkjd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejvcewjn.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmfixpmv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hcmniqvn.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ysnciuwx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3paqkuqui.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3mszsopsl.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ehrgaaio.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3burueqgs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3kpasuvea.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3korzgzvs.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qhxfweqn.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rxlsnxif.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jzkhkzik.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3twuiagia.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3aluyhgfj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xlqkwzvu.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3evyfbfuh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3swllhhxd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jrupnmbe.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qeonqpjv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dcltngpi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kdrxcfrt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3hcrxlebl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3htitvfuy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqkbnycg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3bconjdda.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3cnqsvbam.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3irxmymdh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3qrwwkskv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3kljlncjf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3cyeeztvy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3zjuvhshz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3gkkertxp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rjrobnqk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3exqfgayr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3uqyflldw.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3glnenqoh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3nntcwcvz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3aishtwbq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3fkbmeewi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3khrvscps.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3nrdinxjy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3nmscecyb.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3agdatxlq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3whhqdegc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3fvbpqscx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qihowwpm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zvymndxp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hbbdwiwc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3tubqhane.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3cxzzibvq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3bzrnrlgj.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3xmcdxbwe.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3adztomji.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3zjheaabr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3xpiwthar.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yvjcbpfp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ntespjes.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3fadvfjcq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3skaoevfi.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3twctkzec.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3smxeuxis.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3jrenixdc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3bufwshhr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lieakmnz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vnfaeeaa.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qfonpwbu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3delajfsf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3utwbxaak.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kupdfzfw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3qeetsvvh.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3zhvatsuz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3bwxksefs.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jkmgceqg.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qqtrbdzr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qektvbdb.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mkbrxrma.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3abhgwsef.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qufvwjmw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wdmddcmp.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3qdhefsfz.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjhjzond.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hjhapmzw.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ujgskzwv.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vbdzpwgf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3kkanhcpf.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3mbfsgakt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gnydjjft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fnivlwmd.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hyfhdeiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xnjxitig.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3canktlbs.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3asmzebtf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztmrbopp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3apczoevq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ivpdgsdf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xksujcix.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3nghdhwlt.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3irslsual.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3usoplxqr.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zbyzbgjp.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3huyvrikd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nffbtjmm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3endicmjy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwnqzguf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ymkzktgk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3jkkxruyo.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ckhxfyay.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3namrahvb.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3mzlfikrz.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3fptofqtp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3qgiwopyl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wsvhnjxd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3lbwrjfnx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ntbvgrcq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3avvurxdt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3lhhhkexk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3hywudjww.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3tvajcwtt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3dbqizbjy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3pgtpbvru.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3aqidyeyq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vtgnbpkc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3zqjalbwg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3efxionoc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zzovoobg.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vvzcmngs.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3cofimnqz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zwlrcrvk.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3bihhjgsi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3qvzhnjca.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3rsbvorsd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3kfeurebm.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cdbxeihy.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3jfvhnrtp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3wlfuscue.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3gzbeumjt.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3dbyafepo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3xkeylfcx.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3asxivdhd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yyqsfgli.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xvwkyeeo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3pjolxtvq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3ojutkazk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3eauvaivp.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3lnjlggcq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3tnmypyuk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3gnrppqds.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3pekzehis.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ujclranu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3pabhhfps.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3fbrkpsno.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3zhbwtzws.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3eaehvlfu.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ywfdstut.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ynvhirzy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ventklae.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zqldgnew.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvzvhcbg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3kofthttg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3mzamikyy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3tdxxfncg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lokoqqgz.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3jvmgoodu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3kkqnrewi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3dbncqlny.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jdzyqcze.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3hwauaxlb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3izkqjyfr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3thbyurzw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3gbycqtxs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wmmxtvwe.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3zjqwcunv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3yqvoldwm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3fbjdvmfi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lkjkrxop.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3birdtlzv.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kxdqwmpy.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qhglcoro.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3jlxabotc.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kdwqacsp.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3uicygknq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3kbrozbdi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3rtzwvlwy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mrxejhna.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ntzyvaqe.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3cjsfscly.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3edehfbbb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3wjejyolj.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3cajwpkwx.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3yzzvpjlo.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3zzkwlrwm.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3hwycyfdn.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xfxwklkn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3koakjzcr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3sgyzulig.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3zlxiipyr.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3zxdysyws.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3lurmznsg.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3xufgtqjg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3odbllwaa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3udzkxifd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3uhhfcvjf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dofrrnhg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsyzmujp.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ywfqbxqv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3imeypgtg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3znmgxxkk.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3demideal.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3enkwtpfn.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ziyewmdz.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3pvzuppzh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3hrajujta.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3dpwxnoea.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3nhuzxrba.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rtamyitz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3dywlorev.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3boaaqdwd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3mjaeswet.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wnpzkolf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bkyutzwn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3adbrfksr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vtaibfqn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3sdrskbgq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3hpvirbsr.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3doyaoexh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3tftzyynz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3eilmogyw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3wqliompc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3oevtvciq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3nvryvosr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3njmvtoeu.html


<!-- 参考信息 -->