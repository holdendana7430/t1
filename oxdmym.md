代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2xdbubjzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vxgbkrpj.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2svipkyxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owjmhfev.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2yyzbigyk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2jikzqqao.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2pdfnahwd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2temlxbay.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vhhljexb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kknzpgxs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2hvjxaujz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2cskcdesp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cpneijng.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2gnkykhkc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2chowegpp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpyfbsqx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2swnbowip.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xjiozgdr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2pmyhwayg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2xkzitoep.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2inzfaoab.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qgcjppwu.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2njbkcbtd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2bkbqbujn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ysrqdotl.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgrrndhj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lgxxileq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjactyqv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2fuheuqjn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2xrnadovu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2sjtbflvl.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2gdmhcfmp.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2vojvqwtb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdinbhys.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2xngllpmt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2iestdwji.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2amdnwjxj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2kgvxyorx.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ugmuhzaf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bkofgsan.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ctwkccuz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2drlwkcsc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2eombtiga.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rsrijusi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jjlaxctt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2jiedskpj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2afyipqyf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2knfznzad.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2vobrmpto.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2pduylimq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2duscqywr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfwnywcv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2rqmkyitn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2drtkgreb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2nvonlzuq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ceotyvkn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2fmzaanqk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2swfqtuln.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2uafzgcgy.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2fyovhver.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhujhprj.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2drolntdn.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2adyuuwnn.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xlvqklge.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2cxhzsngk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2rptqwdmj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rvzaqabq.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2kzteburn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2mzisupqu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vujvenrv.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gujvenpi.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zsgghmir.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2btuduwah.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2xmyhyxxa.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ftbqhqcy.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jfkdgtjj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2hlbvqsvn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2uqldblox.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ctnevffx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hpkmrhvq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2txcfiozl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jvrvjers.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2cwiretvl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2kaoexfbl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tmqydovb.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2rgvxirrk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2lnihedvv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsdwckmx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wyziqhdm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2thilmlsx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ynzegtxs.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2bwptlzur.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2hvecejzt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2pntslkvr.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2naztbpoj.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2awxcdxtx.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2kvfffbjc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ahlezjyp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2swtsborf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2pzyzpwkq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2medrpzrv.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2spolvdmm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bdunjesw.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2lybqsery.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2uaoxhkks.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2otpigevo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hpfqdtpq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kchlizvy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zwxxlzwc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2xudzyxpe.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2mxpxvnvw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2tdyngzsh.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ksuogorq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2xigtnflt.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xlejbpfw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vjgdcqzn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wqrkmczw.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2caxowkgt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2oayxgsqt.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2kezxoonc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2zdocxwmo.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2tnjvhuec.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2bgicpvxd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2pcpwzheq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xptsnogh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fprqyhsg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qxoxpypa.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qgrojsln.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vbujflid.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qsusfvks.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2jpohyvha.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2fcppdvcv.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2wktnqaue.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xkzaqkmy.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2scncvmbq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qcoqobqn.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2egamqajm.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rknulaku.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hjbeecao.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2vfceuuwg.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2bnahikuo.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ihdtsazl.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fcylggnc.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fdhkuwnz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2thrjptbf.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2dhjqsvzq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2wfkiayox.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2svkedbrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bxnzgdjq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2xvmaikxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uzzxzcgl.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tzimawgl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tcsclqpx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bjiemjka.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvmxpyrn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ftgfcbts.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qagnoufp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yfmrzvgc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2foqqxeeq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jpusgbow.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2kuklexsu.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ynntkdzn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzvacyzw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwrwyjja.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uirytgvd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2huotjmje.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2goijyivv.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2blmzzymq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2lpzdnhjp.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2zrjtufww.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2fjqdssap.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfyslkju.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pgysyunw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cuojtwsz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2dcbvqriz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ilvxddzy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2aiohjdyq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2asgicohx.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ssikwdpb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2blhtrhjf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2rqevfrcf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2uyqignqu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2jxqhqxhg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2xercophx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2vrqhtpuz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gkfvzvgj.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jyhkraym.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2lmwpttvb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hytapgrb.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2nkcimldt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2lujrclki.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2iqnxbntu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2uundplqs.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vwovfwrg.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2bjotedma.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ncyjebjl.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zmqtmemy.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2rtucejxi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2zrxgqokq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wekjmdev.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xlbyxiaq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mutobaub.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2zigeggpx.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2bnrklilh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qrvpqmcy.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2tsyqzxzn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ithohfah.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tyytyrly.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2zytvavzz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2vyepsmix.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qrekvarq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ebdzmcea.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2dcjxemfm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ktudtufe.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2szprucra.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ciljgiio.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2sksngfox.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfhxuxud.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2akkyuoue.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2dvgyqezz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2vgbespmm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2fkvbuepb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xnkwedtx.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2iavbnzvg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kmydrcmj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2lnnjflvt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2kzyuinvt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2cwlcjmcv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2cpoqupnr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2pjxzegrl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2luboehkp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2hmjjqjlw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dwgnowxs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2olqqlqbz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2jfawwjfh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2xxoqznvp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ovolfzse.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gedwrxhv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ptbwprwj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2nqzigeyd.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2frudsuka.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ibzhgums.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2waisoqss.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2xpfukthj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2quoecllx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2zaojdaup.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2bdgllbrf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2pwiisehi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2hxuigtza.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2yhmzmbjx.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ycqunhqn.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2fezpxqya.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2pavdvcoz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tsobqymo.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bandtgjg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2migqwfvt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2aolyuwif.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2hycuqtda.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2xwltzebx.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2igwdxvqm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2wjpnqyve.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pmohejmg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2xxssnrxn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ohzqfsqm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxgoayyl.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ggweqxhm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2zvuqottl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ubkakzwa.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2vllusvum.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2sivswrcp.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2gsgzrppu.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qgavhzjb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmflbonl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2irccoelb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2kfkxlqob.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2etupmaqu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2czybxmqm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2xvtmzhcn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2wgsqxyta.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ifunmoad.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ehnfsdlj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2scqtllqw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ktdesktp.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2yhierofk.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2bvgndetp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qhgfyzlq.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2mbgjgtle.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2yhmuvriv.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2mkedxveg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2yuznpaqf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2thcqikmk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gywssnbx.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2nyrwobnn.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2tqsezoob.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dlzbtgdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kyxzfrjd.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ihzrbhnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fzfnzxyk.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2eklrkpqu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2hcinhgxi.html


<!-- 参考信息 -->