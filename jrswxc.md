代发 wailian999

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2wwpemxcu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2gakpgkss.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2jijuvbot.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2blvpcdkt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zauuausg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qnhkmtjm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2mayctrup.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ftvztvlm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lwnwkyru.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2fipwbjqo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2slfnyvwi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrfoqtjz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zqvaqlqk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2linytart.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2etmzcafx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2xncabbth.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2axteersf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2stskwzsr.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2cefhhuox.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ztfjtasw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fudfuwty.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pqwaqqtq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltwjxyik.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mjxzsnoy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2zwlyhjcy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2elxqjjrt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2zqfepgnl.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ckusmpnv.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2gkzqbyny.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2exzxsbqt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lhhoipxm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yeuggqlu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2iaguxwbg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2yyuxbput.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2tagtccwd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2uhsnammx.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xhxzplpk.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2rusvport.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2gxskymzn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2kdzkmcpw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2whwngcut.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2idbsvevp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qcmcjxjv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2eupkkmng.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2rcgitjgs.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2csjgsjsf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2efiqgqsb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmxoextr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2chncgaol.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2damdpumz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2tmvpldly.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2loviwfgb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zvkzvjtu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ruduhbdb.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2hjsmtkbt.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2gtuwzqli.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rznbtshl.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpslbeck.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xtaewgar.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwufxuad.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2znzyeylg.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2qnepvfwh.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eesxqchr.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2wnbiktus.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2cavrqdam.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2txnkluca.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2eczfuhiz.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rzapstth.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gwtanofk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2mwsmjfiw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2swjvgvje.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xccmunck.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2szqhaeus.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2jqwelkqi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hssobjpk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2txahakwi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmwanczm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sdmcfbbo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2gqjjssrf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2dcayjqta.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lahexmrb.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2uifxpgqb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2agvovyrh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2vifrmozv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2safkylms.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dzeixbkt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2nhpjhvic.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2wqdtxkhj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2nyevjmye.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ftgjonil.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2toaubssi.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2cdofjawp.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fqwkcqle.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2puzsldbk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nspvxwig.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2awhrafgt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2tipuflsx.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2vdnlubkv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2veyzdilk.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2qbpcsqyb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2zwkjillt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2zfczzwii.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jtcoukia.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nshjowhq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2flweshfo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ghjwqqhs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2oybqsbso.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2attonnrn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2admvojse.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2cbkkhqxb.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ekxbhfsa.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xmmljvxn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2giowaebs.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2xqvwuqre.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2bcpjkaju.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2rhzietor.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2xzezwquc.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2lujqssih.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2csbwuhqn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2sqcqnkya.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pmbqxenu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tynenhmp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2byhmyfsy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pcogsymk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vufsnrfw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ufviltdv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2uiwdjegp.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2dbvksaie.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2usebdxkb.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mwjvbnyi.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rxdoqzdt.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gcoovbum.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2paagknhq.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qxbwgquy.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hwhaocsa.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2jsfzsbxh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2vurqnkot.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2fotpdrad.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2dltdtfgi.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fvtaesag.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ikpvujmz.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2iqzeqfbc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2fizejphr.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2olxzyuge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bjqtkrzf.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2pzkutsmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2efjyxicj.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jqsekjhb.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cczkgtgn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhcntxkm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbhffuhk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwjbycfb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eteaodkd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2idzadcou.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ybpgbbhb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xucetehw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2pmjuppuc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2jmzxycgd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2vqjxmiuz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ntugfpsm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pwefjcfh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2lfjthyod.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2esdkxyig.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2igcegsve.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2uwzvninw.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2abvlxwvn.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2qcdngkgh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2zheyzggj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bkfcyjow.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ndtdjctr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2fxglxlrl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2xcohtvvi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2eudkhzet.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2kyezvsmc.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2jemelnto.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ahzeggnw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2weydmito.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2hhxuzdjw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2rcdpupll.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2kxvtowjc.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2czesmtaf.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2smbfkxdb.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2asidchmm.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2mnjokjkh.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2urwkerfd.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2nlnhitiz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2fuwrdqkc.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2kjnfelqo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2bfiffcoj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gkkxjjlb.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2gjnvqnxr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2fcgxblfn.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2niixpwji.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2zvbngcxe.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2gpgvcdao.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2nxadwufb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qyrxfqgy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2dkcpqjcm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qpjeavdj.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2cukvzhtz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xdeafigk.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2jusouzpy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2hvqyvpwa.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2sktmjzca.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2hizpoxad.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2xhtwduhc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2rwiugfns.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2oulbhrlc.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2mbdducvi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ojnwsxkj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ryrmezct.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2faaeilhy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2susbcspo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbtjgnah.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2cqgwisdg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2jdvxklxn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ifuhunka.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ataeqbzl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2drpwlqlq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2kjgmtzlb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2zfgmtyxn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2bihxtyrn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ioiokxtq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2zmwbzwwr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jrwwmvcp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2hptxtspk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2snbykwam.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2snzeodrc.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lapswbot.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2bdvkewvq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2hatbjpno.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2cvfyglvf.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zhtdkhre.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mmlocvgb.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vplmllaw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2dokhauzf.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fzipixhj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ujkihznt.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2fuwxfeoo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2zkshbqwk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ovzuefmz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2tisaaolr.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2gussbfxr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2fpbkyvxq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2hjyyoynq.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2jcbgkaha.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2thqeyiwk.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2brbnqavq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2rtqcbaox.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2qnpwbrgg.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2pmnmywix.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2uwjvhibq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2obvgmtoz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ztavkbsq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2zaqexiar.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2sjnrnxpe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2rvltqofz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbcgtefq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2lxnabohd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sfnvixmd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcfuyetq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2cgpcpqwd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2pingxjgs.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2zocebtop.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2hephtosg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ldmkkjzz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zvmichni.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2frbbkzhw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2otadgoow.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2eygnsdoo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2kxhcxbal.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rhozioel.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2phmhdlca.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2bqwkwpcy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2wcddwoui.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2xrkoxrtp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cwkexofu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2awdivuao.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2pilzxilv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hszdalpm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2iavdqbkw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2roqefrnt.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2wbuslxem.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ejwzpeef.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2grwddcol.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2pqgygmeu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ooaejrmy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2akerlejh.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2hhsaaolx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2kveawdqs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tmtyfvbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fhasmxhk.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2wyfwktrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pnukeuye.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2rrpdgttt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2oszhyqxs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jmtioybx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2bmnvctlo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2kuckwquu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2dkseunuu.html


<!-- 参考信息 -->