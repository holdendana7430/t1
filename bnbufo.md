代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3thwfekdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yxuffreu.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ytgmvppv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ibtmtcpn.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3znnynczo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3vdqaovho.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tldcitas.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3erripgay.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3liocssid.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rveqwdxw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3mqzpoosj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3doprhqxh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rzeqhaiw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3jharutew.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3qwhfluti.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3lakqxenz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kvaheipe.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vzqfurjj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lkufdxew.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3jaxxekkd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3zarhaxry.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bxltobjv.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3xwlqjogy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3dflgfgzj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3edqzhbio.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3esifxpjl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjeyaele.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqyzkvji.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3iyluhysl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3vdcneeys.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fhftfbrv.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3nbrshirn.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3gokhuvpx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3hlqoztwt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zjehuzdj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ghqxmwcb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mawkazxi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3onciawtc.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3uwfxviwy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rizlzvcs.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jsstjwub.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3plkhbsti.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3wixwhved.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3eclrohpi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3liahjycw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjyomhge.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hfdhghpt.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3kxuwtnqe.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbzkooym.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3tblbqonk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3pflfyfkb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttsfvqqo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fluewptz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3lmewijug.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3czcgyver.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3hqytgahy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3dwmeswiw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3nxjecoce.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3mckffhik.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3tsndcqbv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3govaihuf.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwxivxss.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nzndpgsx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3weqyccnm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3qtshuxue.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3wvouesqv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndmtbztz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ehvwskoi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3rjaatvzh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3maatpelc.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hcypjkmy.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ocukphhh.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pakolpnp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cxkodbwq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3xinlrjzo.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3adxnnovf.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3dfmhprhr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3blaulxbf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3putgotmj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3trqvadgg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzlpsvzj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjvwrutj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3dbipwrbh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3yybzruyj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3eoddaxnf.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ivhzfaqt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3nlbgbsvw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3pldzdlby.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3dzimoppi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3jqxbyedh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqyrnzey.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ycscxuer.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hxsbanfz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3djvlbhlx.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ymuuvtmr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3glaysqse.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ouwhojsi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jmifhyfl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3toicqohr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dnptgkyo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3iasvslus.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ywxtkiyr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3bifqxgnx.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3irvgoblt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3mbrkkntb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3qxgzpzve.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3auvsjlvy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zrqhunyf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ihpeyyeq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3qgstpynv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3uyllvwnf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3udygupox.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3otsrbuzm.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3kbiskcft.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3llvjtrro.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yputtfpn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3mwukntge.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3elyxbiis.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3mubqkkqs.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3bypfuroh.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3pboolthu.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3pdkdzwzl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3flfyzzxk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3arsxmqzb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jfhxcosf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nijhjpep.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gvnxgqpq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3mjzurcih.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dcojjozm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rfvqbjjk.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3gfensvpo.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3yjxusfyo.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ugzezivj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fxsoyunr.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uymyzsjw.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3naouqlli.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xylcacuy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3psdbkaga.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vcyjqkud.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3yigajedk.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3fdxjzwfv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3uqfpptjq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3saugxfrz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3qsuyibpm.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jtgxinxl.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3oirtbjlz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3glrxyoqp.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3fmkjzjkv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vlqcolym.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nmdgspyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dpsodzdq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wuoqhqbv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3mbfpufva.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kduhnfmy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gxdwwjqt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dxovlcgf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukunfxql.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tecvuhly.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3cgxhiuox.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xuoyiwya.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3iqkofjfi.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3szxkxluu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3twzyoieb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zbynbzdx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggryboip.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3kyqkizho.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3zybtczcu.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3snpcwybp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3qrwbttid.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3xhpvcdkr.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3kuhkemiu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3lqebiogi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3svjfpibq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jsucklgr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3usxjnnix.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ahvzvvxs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3kfkccmbn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3acvanpmr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3zgalwbpc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3cgtpppzz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3olvvypwd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3drphvlal.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3eueptbsv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3upxotxxr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3jpdgctdq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ygsspajb.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kpiosapk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ngkkhbsp.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3aknvprrr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3fnvlquyy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jlsitiym.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3dgreytnd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3whjlxuvf.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ogbkujxn.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3twefajbv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3grinatlo.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3rcngrcss.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3roayalvg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3lzrdwahl.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rbjsrvop.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vsldziyf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3zawxfcig.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3hyevpwla.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3yzcrlvud.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vieydnho.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3lugjiyon.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3rapvytnz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ykncopwd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3awsjeqxv.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3jbviudrc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vfjmozjg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3witsfchy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3usbjfjtu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3dgkptydq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3cskedljv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3tprfjsup.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3tzgddkwf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuzbtjbz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3loxollcr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3lpvtfxki.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3xrkcxeaj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3iiwxboyc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixdcrayw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3svfklldd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ibbhkzdi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3sygrzyrr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3uvqrrhai.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rcoczhzi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3gfufdris.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3kmhrxrad.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wffrzzgi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qrnbfjni.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wiqyteee.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3xtdlpyxv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ruybyule.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3wwidprvc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vohxmyvq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hathfsdl.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3arvpkcuw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3mjrvgmum.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3coozxqej.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3mmqmafpg.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3laabrbzl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3wwiudina.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ohwvhxnp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3vjigfsnf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3lwaimuuz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3etkhohsj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3gexlkyua.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3yjczoshz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3hwhjvtxc.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3xnhjwynz.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3cierfmbe.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3gvfxpvog.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3vfaufmba.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3zkeefodj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3cjyggvbr.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3fxurygga.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3wnyarqah.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3euihoagi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3nzujqbge.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iodyzoqz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3dhtsgcsp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jimobybc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3buleswrg.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3lzeqtbzt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3prlxvnxx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3llqcrlsd.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3vuwryyex.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3cpdwybgy.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vdqzyadg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wktkcbmi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3meakbyud.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3tjpdxmho.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3oiurssei.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ksxffvzd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3tabfuqah.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3tklwtpul.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3zmycsofv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3jwkxaizp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3fgckvfur.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3cuxqdozp.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3foncqwcq.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wvsfovno.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3wdmbbnfd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3untmyuwa.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3trbvvvim.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3brwcndos.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3xolntfyp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3eyznbnqp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3arfputjj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcruqbel.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3davoavqm.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ciacktki.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iadpdhch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3updxnwql.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ttabgxhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gnutrixz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zdzxoeve.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3fpoxtzsx.html


<!-- 参考信息 -->