代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vnxjzrng.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dcbyklrg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2opnvkplb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2wcxsqest.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2llthvvkh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2prjannfd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ujyjxasl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ffdfqhpo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lsubgzmw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgtqdauf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lpvjemev.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gxebwthq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2rftawhvz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2mhogxazw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2zkzdmrxf.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2hkrqacgl.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2zobpqibt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2jzykzryi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ohbeovwy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ixtzbvlj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ggmoqelr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2pswfxijr.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2fkzuojtt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2jofkamqb.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2cpneztbz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2xuznokdm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2wrgsiuca.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ezcvvgfi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgsojyey.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2flheqpwo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2nhjjzvmm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2myhtsasj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2prdwbvpr.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2gcfzbdqy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2abdvpgyt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2dgjwyija.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2jmcfysfg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2svndzmoo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2gcknjugw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2xduulmow.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2iaobxqix.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2pimdnazl.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2aoamgrnc.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ifazgnfk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2chlujkaj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2invcnjur.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xddmfrvp.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqttogay.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2dcispehc.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2zntetwvw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2uxgxdwbn.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2zccyqwxy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2wrdtawmc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yqfiecqc.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xrmzuovp.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ddidfxay.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iegkmpex.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kcrqvwml.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2zjjspmsv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cmkkqdpe.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2fntspyyy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ygwvmqtv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zukgbgip.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xylybskf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nnjjjpgd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2iuofvbyv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2bzhcxxze.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2qmlixjur.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ezozhbvt.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2jziotdbl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ihiuraem.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ktvpqcit.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2xtszutah.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2idicnpod.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2afmszarj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2pxwjkxey.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2zwbpgsej.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ycwunkhn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2vxzkypwm.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2dgycfkks.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2suzmgtyq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2pnzpcbsy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ttdcbneh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2umgatbws.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2tezwrdtt.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2gdtmoqtd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2zybfcues.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2sgwlgbka.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2fhwjqhnz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2zumyzpzl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kvxutxas.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cbcsbtqe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ydcothil.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2vwvnjivn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2qowcoytq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2tfaihbsb.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2cyezydbq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2nhjriovz.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2alogzyqx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ccsqdixi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2oipwrotc.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2evgwnuip.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2lrsckfgz.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2hpvuvxoh.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2jroromii.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2fftadqvq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jvbxodkm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2nxkxahzp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tgnwvvwo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2oxntpatv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dvcvtwpx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kmougglx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zkzqnjct.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mvhgkpic.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2oymnrlqu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2hnmvltkv.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2zumzksgx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yukwmtas.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2drlikqfw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nhjzqnqv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kfuccooi.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2obhrhcrh.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jlcllcrg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2kwrtajip.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2kddjdvys.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2lqqwabae.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2gjbodlcl.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dmyrbxlg.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zhjidlxq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2kbyhahnb.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2yblrehbf.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pvzvmsni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2prdflmtu.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ntrqicjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eitejwjy.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2aeupxphm.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2hefwgmnd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2htmhowwm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwttjywx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbmdwldr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hjzklpvy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fbhfxher.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2jegcsctj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yemlqrkm.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2xmgovote.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2trcvbhrb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgkzyjwq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbawnidx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqicnvcp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2xpfurdyd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2tlvlgenr.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2olrejaem.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2jfjumzlb.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2zddebqgh.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2hhjfssmm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2qoufhfbv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2fnlwisic.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2azmvzlkw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkvynkij.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2dyuotltm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2povbxzrr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2zyxkdrfs.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2hshmksyx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2xutfcaye.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2muvdwowa.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2gajbzjsy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2tdyjskoi.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2kwwascrz.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2jglfbvfr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2idoukwmz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2oxddkpry.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2cbdwfmdh.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2sacsshnp.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2tkmpctjl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2zbyrmvqc.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2rxexatby.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2jptskhri.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2sdfzqgvj.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2panhhxfy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ypvgvqps.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2uinmplhj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2gatzhvpp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2utmosvdh.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ynoulzax.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2elvzrqzy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2orairxau.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2utxfbkki.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ugjpkiud.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hbgpmimr.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2lifwxyye.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2miqethdz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2irjzrldr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2phvnadvt.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2qlejhqsx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vfzkazmx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2esknjlzj.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2sfqcndoa.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2segwhmsa.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2lpedmrzl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2klyagupk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2qnntxnsc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xumlldeb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2weadyicc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2mvbhsyir.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ddmftngh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2xntpxuwh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ayzbnumm.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2llogfigc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2yqhsoozi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxwcyylr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rlnqejjr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fezuhkde.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2sacfahuo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2wzyyphxv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2pvrvqsrj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2yzrpbzip.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2fitbufhg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2zejgpsxi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2flkfqtab.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dfkhiaxm.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2giutjmto.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ajyjaamm.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ybjblchm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ezmcsomw.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vfszgmth.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2swccdtqh.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2rmhshkdk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2agumseek.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2athopgfv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2iqdavkuw.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2miknfwam.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2gmeelxbz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2bpygoust.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2rgkfqusb.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2mevjqpiy.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2fzekqvli.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2esrxohsd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2gbgqaoqq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2prywuarx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2trexdtbv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ehpnkuyj.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2cxitqnef.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2mvpulznx.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2vmhrrgyc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2xthvsfqh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuikaaol.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2rvuogchy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zwyiiirz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2glfyxwvx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2zlqbipwh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2hstrnqjn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2mhbwsnmx.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2jqrihuqp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2jsbjageb.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qasekqso.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nqsafnwq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ofvnvgci.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2rsjrqygy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2qnnmqlab.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dfncgkis.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2vmdzxkkc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2gwfsxwsv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2otdurfao.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2wyigshji.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2mvqzgkan.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fcyflahe.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2kmvhqlzx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hmaclyuj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2spnlnrmg.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2feepwqcb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2qpiqgcly.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2sscxcltt.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2fyeitgoa.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2lfjjlcag.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2zbucqudz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oyjofnpo.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2dmwjwuzt.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2naqwvoxn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2axxzqeun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lzvgrgdk.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2wooxvevh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cepiexrb.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2etmimedg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2aljfrvmc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2cnbcbjqe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2phrdbaok.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2omlijcqp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2rgszuamq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2pfyjjeor.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2obpxmzgb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2tgdadwui.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2sxpspubz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ckrpguog.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2hqbxrfao.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fbrtmonl.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pqzedzip.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2wuiklyzq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2lmxzkudf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2dmrbbnck.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vwjjhzgd.html


<!-- 参考信息 -->