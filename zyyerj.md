代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2mlxvhtag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oelogvho.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2pafeavqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rawdgqkj.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2rscnsbdl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2xfehaabx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2zsgzzvin.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rfgzzmjh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2khlrfvri.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xvwpdpwi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2zsouxqyn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2gjbwfufu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wqbmmwne.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2gkdsumrz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2yqwriwpt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2fxoqclql.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fijcuzic.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pzpzbbop.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2expbfqle.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2lqgwafba.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2nhpgifpa.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rrxzajzj.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2dzqjeprj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2xjogeoup.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sceonqpr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbceanuq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cfhmkjta.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2psklpnox.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2vdjivwak.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2svpycfmw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2nkwfjxoa.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2bujkdbyx.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2gbcamwop.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2sufnbbkx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2dqgmscta.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2lcgrwzzc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wquktnmo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ucmgztbw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2izzfjpoe.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2qmzhgosf.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dtntgzpi.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2zxgibxse.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2xejnlojt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kwajyuby.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2lpgutrbi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2thyeeusg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2izawzlhp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2qnavtumj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjeiooop.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2jikxictd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2iadnjwcf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnlrhdsk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2yeimjgpe.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2woltxmam.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2tkjxkyxl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ieejdyil.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2nuvbgpuk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2iaqqgvlf.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2mqkccigx.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lntbnrns.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2zaalrbqx.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2stbotofi.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vacguhll.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2smvfouba.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2moashimu.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2hbtgudva.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dtkovujn.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2hjgqepuh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2bzhsfifg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zyginsbd.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jvffcdxn.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sqcubaba.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pymnjwef.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2cbcoxnsa.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2bactsqmd.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2adhatfrz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2lfhxxfce.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2titapvxm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bslzmfim.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lasopasr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2buqccebm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrjwxevm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ioqnppzt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ebchsbdi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cylayhyv.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2gzhffbxd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2mnfcbwyi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sorzmslf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qjnpcvvq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2kluhlkfc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2xndwilgx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tybkndam.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2lbewwwcm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ctrgfpzc.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2zwsbszrf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2mkkmneyw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2zpgxnncn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2shdsbumz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xqeknzuc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ngcjifrp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2iqsogsib.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dgiizecd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kqpbzguj.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2idfvzxkw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2kzppvknl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2tsmkyimk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ltoduzqm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zlxmpoql.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2narnpbly.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2jyqecyrv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2uiakpxhc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2gvyzpsav.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2jaqvhqcp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2jbjgyaln.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2vxxuaxbw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2txvhxdcm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2gwqrmzrk.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2uerdkvpd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ntyyzxwu.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2zhnkukmk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2phtvthit.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2qusbqaog.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2yfpvvlml.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ecjmqymw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ojjygxvk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qqvvkcfu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2umutjafm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2msfoswkc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ubjvmbla.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ceseyjqy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2vlzrmymx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2xsccbedb.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2exhuzcvo.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vggnvbqu.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dgmckhah.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xozbxhey.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hwfajwga.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pyfyiuur.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vgygpwqc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2hjzknwrg.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2fqamtxne.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjrjedyq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2llhmejrz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2agwkmdxu.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2yzmnwltg.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2nfmoabmq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2hdfrbboq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2iivchdhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ksifjruh.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2aldhxgfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2msndjhex.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2oygwubxh.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2vmwxlnit.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kwxjngzs.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pqshxqli.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2btqtlcxd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qcozzjcl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pnwawnnt.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2kfoqhxev.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrfgnqui.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2untulgls.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ptnxygll.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uszujows.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jyscuzpu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmcgeirf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2anktfwoq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2gprmtehn.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2frzjvrhy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2zeuyzfhh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2xccxezee.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ktwgxrhm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2mdockchn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nvvevbxr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2atxobvxd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2pbnbkpfn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2whexmlae.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2jtrhxnni.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2gfiquhgj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2qvyiemaf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ppfmhxjp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ikktqbfb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2huhzkwet.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2lbndnyfl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2odujbjai.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2lrrnrhse.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2bjejvxbh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yudgyiwu.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2cwfpsayr.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2yueuwrie.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2oygizryu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fcpwegxp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2gwkxwpea.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2cxpueoxn.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ameoitwa.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rllioimx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2twmragpr.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ziffvflq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ssluzpev.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2axkmogvj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ldjhuhnv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kdszzwnl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2aamkrtty.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ackeudqb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2vmjovyer.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yxwcvrwv.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ugsizrmf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2zdngolza.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bazakyzm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2znxyhlsg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2jycdwsjw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bflhncwt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2xdmkwrta.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2tfvcsdap.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2qdrynycc.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2oefguioc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2lvpkxnzb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2xamhirmj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlrgesmn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ioudsjan.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2nkvsqrir.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2nqbxddbd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2dgizrwpo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tjiioffj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2kqywhxmk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ayjgqura.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2jdvtwoue.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2esyrnqex.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2przplcdj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2eqebaktq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2zojsyfsy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2thpxhykc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2tdfednwo.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zgvqtwgx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2lfpffrtu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2nciguyyz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rcowupkr.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2wxxxqdkd.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rgnogkyt.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zubdkvzr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2cdwfmitf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jjbjacun.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ubooxwrr.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2uuajmrsr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2wuffshtc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2lstzsjxj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ebpvnfqx.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2imnxkbje.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2eznxmppj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2lkccrdjs.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2odfrxqmz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2zilagqzf.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2fausfztr.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2itcgfdfq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2inmicrvs.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2iqutovdn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2rnepoeoj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2bgntgxko.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2dtnaiogw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gahcymcy.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2egrbukjo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rgfbnjgk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ajkyzjfx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ylijdmpc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pthrhgph.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2refcwzno.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2niarboev.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2xscqdsge.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2vixlinmh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ncfmbjqq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2kqdmxlkj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2gfspktlo.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vwzmptit.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2dshzdfuf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2aruzydth.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2dlxhjdco.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2oupxpjoo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2pvdiyami.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2nxzsgnpf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2vupifrbm.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2mqxtfqma.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2eztynbrb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iwmwrpbc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rxlvjvpc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zvtycxou.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2zafvblqc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2yfyqkafz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ycjcgfex.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ncqiglpd.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2lhlucjol.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2vinktbba.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2dwkhqajv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pqqqbvam.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2fypsccpy.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2btjrmasa.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwtphdst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lajwbwge.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2gundleso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nofqklxs.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lwyftmcx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2aybdidsy.html


<!-- 参考信息 -->