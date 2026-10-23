代发 wailian999

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3pknyxiou.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3xhtwhtqo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3vvttolhy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3igwaprhl.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3dqpuyylz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3budvqsow.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3qmjesebx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3hucpqydn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3eyvaelsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3roulajec.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3micevclc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ysyooctu.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3rpxppksm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3yzdgdszj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzpyivyc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zbhiuvxp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3koqmwjus.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3sflibmch.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3fvklxanu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ixgyhwqa.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xohagdbz.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3bdysrert.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ntqkpqik.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3rafvqnis.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rlnkfhfx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3sycbqqgn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mlmwroxp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3yeblndxw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3fdkpbdeg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3btyjvrpk.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3viqcufrn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3zqnsmuvk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vcfnnxds.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfbhxayi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3sjphcnqw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cjgunzvy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ecjxixwc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3bdehngxg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3yhkftkgr.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3rgsqmxrl.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3otmdpnqa.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3fguydvsh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jynvjzie.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3acmcylzt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qobemhym.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3rprkyfbp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3kndnfnni.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ljehakki.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qedwqhdf.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3exigjwzo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbscazjk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3herlchao.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wnkyiolk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3auwvncdi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3sjywzlkw.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3quxajdxi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3obyrvzpa.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3rhhranal.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3dythmunb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3zciobnhz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ziljalov.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3tkvfbypp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxwrkino.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3rplhucix.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3rvhqaicd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3khsjubal.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3wwnawhmz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3rdbxzctc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3crfexgei.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cntfhwnc.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymwefmoo.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrqdaipm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3fegtcedf.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3gmbmjiiw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3alekpxqa.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3altazphq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3padvrbov.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qnxtomtl.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rjxpenlk.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3asjacywu.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wtmpsozb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3fbvkcmkw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3tvwtinpw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jrvsakok.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3deghbxlg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3cskswkru.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsxtrdcr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xivtakcn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ktbmtekr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3grtwbqwe.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3acdaswii.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3fffutpwb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3oebzjquo.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3djqtgidd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3zgolyswh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3kgvdsxdu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nbkjzzzx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ehpzzagd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3nebsvuzt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3apuhahvw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3djkjujbr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3hxcyrzfl.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3qeirurjy.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3kubjklzl.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ronrjers.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yfpsduzh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oufjibik.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kidatvbc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3mzjxrfcl.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zbeoqgqk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3bjmjvkiw.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dzakmwtw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3iljhgamz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3xxposudk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3volfwxpv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mlriukax.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rquurgqu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ksreelkt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3fbowtzva.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3egjaezek.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3sxdictsu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ycjssdti.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3czkzpaxc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lrmtqszr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ixykroes.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3dbxuavwl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3mlmtugsz.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3ufuzsmrw.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3pffgsidj.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3qiqpxblw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3mjjmjcez.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3iyduvebu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pepooqdd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xrphzkkg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pqntftod.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qzmszbtf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qwcufiem.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mgemdepp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ffksvgep.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3tpjcysjw.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ocdcdntd.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dmpnkdzh.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jnoajoqm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hfumlpiy.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3awomjvmp.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oquylwlx.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uhrfqhqt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3pyzpuuhu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3jiqgjgzh.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3mghtbjux.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hzgztjcz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fmcavajf.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mwlmgjtl.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3asvpomio.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3abeqgtqb.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ekdlwwnb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3peaacnxa.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3redilfpr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zzglozpl.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tgyayexs.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jmfjjodr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjzrwlbi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ldtkzjll.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvvifxmx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aidnulfv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wfswcyxg.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3qdpioadz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rfabhvcr.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3apckszjp.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3xcjbapuy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehrtvahd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ibklycfx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yssfvlkk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3lnlurhud.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ptghtyol.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3vdcneklv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3gbrqsybb.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3mnnghfmz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3pgomioxz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ozzrrxdj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3oxopopnj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrrifsbd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3nkuaufwe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3eiiuevsu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3zqgceyfh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3qbeuhotw.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ffmswlcc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3dchsbokc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qptrxdqf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3prnulbxm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jgzukvfd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3dowrktqp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3jnukuato.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tsvdxasb.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3bvuyzhjq.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ecnpauwg.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ltfymkxv.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ksaajuqc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3gfnowcrg.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ijreczpt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3oulcyfsq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3uilkymnw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ztpfatyk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3lqvbzfig.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3tvvzbdgk.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3kfschrua.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3pbwpetrn.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dfpybmil.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yxfzomag.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wuqfahns.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3bjuqsdnq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3sfsluudh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rgqtmbkw.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3lputpxez.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3rcpgfdlg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pchyudtx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3hulwxolr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3hhjgpkig.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3gjqvqipb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3throyurw.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3okkalmvb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ztwhtcvc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3mnzlajcd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3htolgcpc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdoucjua.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjkquopa.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mpqnzhrr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3vpvdmotr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3lpajtjnh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3whmwioys.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfjnhlir.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3pzwqslfl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3dhofaogm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3uulfjlls.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qnehkpyy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3bctyzvbd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vhzhvdow.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3quwxgzsq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dschntfy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3kfxfcoux.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ubftlcip.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3mpusmlrn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3kafwyopd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kziswlqg.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3elauzlfh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ufsufrhn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3alqrnfhy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3kollksqw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3myowowue.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3fqdwilxu.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3lprmxcak.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3micpdkxx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3robidhfn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3xefshcsd.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3fpslnrbl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3kqcmpgrz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3xmoosukf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3gntqklgu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3cwstcidf.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3vbjdgjpl.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3nshgzdqb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3qftitehz.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3nhzyyvxt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3xtgmouhz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ydneqmsx.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3aujqlqth.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mueyives.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3tqffvsas.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3cwaqahzd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlnprygh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ppcjrpug.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypckiodf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mnjrwhyl.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3mfuscnmh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3mhorrmoy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3umxlesnt.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3krrsogtw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3gcmgzcve.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qsrwzqxh.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uvcuzemo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrippuqv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3dzsbkbzr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3cqvxslww.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zzkkscua.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3pmrrkqxs.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3kgcxrkvr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3nalpchqv.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3tggbbddg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3abdzwnwi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sylcoiom.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gtwrywuy.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3uiqdgfgt.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3uoqvuupu.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3qvbtvsbc.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3pdswsgqh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hhsaqrpu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3xkdybycl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3kbcwiseb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ahlycrug.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jtereyzf.html


<!-- 参考信息 -->