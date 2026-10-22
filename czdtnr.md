代发 wailian999

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2adhyrkwo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2smtljavv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhppayro.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vkqumdwp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dnaeslev.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yhartkfz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2obfcrphz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2wouasdsy.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kcsbxrsf.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2tuptaxiz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2wfkigeqi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eohrzllf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2esxzpadm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2swxjsoct.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2iyxdczgc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2sodwloia.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2hoxeptwv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kvwowtat.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2farlyrwh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2artrasct.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2onvootgz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2erocrxql.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtrnztwn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbjdqtvy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ovdxhtdp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2mbfskghp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2rqqfzbuc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hvnpnqrf.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2enswazzi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2bwronwqs.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijamowiv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vhdfrvvx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqmexjde.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2hlljnqny.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2eetumfxg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2oyqgfaxy.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2lyowtrit.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2dpgwwspt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgdovxzo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2sakytdym.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2vswgwcpw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bsbzomoi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2qeimbdcv.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2pnyefpqd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fgpunncq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ycasaltq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2zjvuxrjm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvjbjanm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2htfoyjbk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jyyltyed.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qrsmebur.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2pmjzzlqy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ppugplpa.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2gagutfsv.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2hinpnmnw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2xlxjxziu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2byxhbzrm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kamnztrq.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgbkflza.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2edczowaz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ensnbpaq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2czruggjk.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2salzpjkl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2rfzasbzo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2wuentqgx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wtecxsen.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wzfzujho.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zotzgdcn.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pxxaeomx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2lnvddxgp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ipydmqug.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vdjcpjfp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2psreiuty.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2kygkpkam.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uiijqmtf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gqwvsfrv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rfimixxw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghgpamal.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2aiucqbzi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2dximhvuc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2efptosib.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2kqioahun.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ctcaqrug.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sblavjlg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dhfpqbxl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2vxzfvtig.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2rxmvwbhy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2zqqxvbph.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2dtirfbsh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2fpoqkdkp.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2rbdeopta.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2gshqrwdc.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lyvlsvxv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vvkhwfbz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uovqqqnl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oilflyzq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2tselcnyf.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2xkfzfudn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2upjticra.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2egrhukrq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2cmpawfsa.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2qpxmsvgs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nwlggpuu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2csmnaray.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zdsbmqzv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2wuljfmmw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2jgzvqwdv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2wbdjasnf.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2beyczjnx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2bmyxnrjk.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2bwvijigh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ytdsghof.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jdebzezs.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2rqjqwyaq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ugqmxmqh.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2eplcdyil.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2qhljuraj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2upakqqpx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2pilnpraw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2gawtsfub.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zchjncfx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yufpxybd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wmdayaod.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sktmycyn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wkcwnwai.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ndfamlth.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2stebgyfi.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2xcoqjjug.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2lyunckgw.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2akyjayul.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zpnvxpsb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fzyxudsf.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2klxhlyxe.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2eatcoobo.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wtpuztga.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ejcrjdhz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ibpqnwem.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2putxvzxa.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fcebcilx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kgsaoeay.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zvmdskcg.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2jqtfolbd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2rqnitlas.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hfjkvfwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2funxdyea.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2drwgcmva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2keistbfn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vgwqadjt.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2divugztn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vjeeykns.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpmhtdip.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2azlmlbai.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ppgtwgca.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ztnafqkn.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2tvgfvjgn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfadcdtg.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2nlypsypr.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2scifnxaw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2cnnjizvu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlucephd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mpttqnmg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2krbfkgzd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2oxmfhqhk.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2wlcaxsdn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2lmvrhgtv.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2pmjqqlfg.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2onvixlyo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2uebczlzy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ykpdvqcn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jvcdzbwz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2wfloeixz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ghfzuxdi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2rrpnkfoj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2opfcycbs.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2lappdsoh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2erhvbfkz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2fhuonaat.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2stkxhikd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2gglwlabt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2osoevemw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2dlwoxffu.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jglrcdsh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ntxxnpjy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2uoujorgw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2qhfycfde.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2vefhpukz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2tbupwnnt.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2daxsafox.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2drmaoyxt.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2itjnbtqd.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2odtaokzc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2zikmwoqo.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2leufanaj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2aeodwlfx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2owdqttzt.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lnxccrmv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2phegmfus.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2wbuiukvh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2pgogjaol.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2fkiauzri.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mczfwnou.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2gveofuxs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2stqmfbwq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2quiwamkn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ryxeslsq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2vvkwuqhr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ugsjaxbo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2nrpdkzmu.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2dvslsrhs.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2umzhnuwy.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2riffjdjf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2gsxsxpbs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2yaokjajj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2yoiiaauf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvrwggwe.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2wgfhsbns.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2wrphgpuo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2aevstcns.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghaazdyc.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2zteisidu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2mxqfcinu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2cisddcsl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2cfucscym.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2cfwwjtcc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2sdplrofz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ftnwukop.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2akhfqwyv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2vdtkeeee.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ukosrrlh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2uwfwexzm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ninncvgb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2tpgsxbjs.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2pirqcybh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qwdvszmw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2blxmtzpx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2dlfcminu.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nwqxtmwy.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ucdzbten.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2yfbcduit.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2wmbexuyp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2emdpvjfc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2jezgpdex.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2yjxjuplo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2fjaowopf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2sgetyaaz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2rshdalkb.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2wmhvukwj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2icdlzmuj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2wuniwbvx.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2umqioblf.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2uplkmrhr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2qwruyhtz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ylhhdqjp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2foqemvzt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zrehgmis.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2dimgjayd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ondjxmow.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2swlfdydv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2digpsess.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzmfsnfa.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyvpkshc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2fyvwnuhk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2proptycn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2vgnwdfjo.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2xhjgsqph.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2qvojfjcq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qpvrkgyk.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2uxbanluu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvnqxigw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2rlabhlkf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2uyqtyywj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2llxrwvwz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2bpciilww.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2quzxahzv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2iqeswsfw.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2rxpaswcj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rfpdbifl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2srogcfex.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2kzkpifyv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2axgvltym.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2gneurbqk.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vcgsaovi.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2edoomuur.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qlhytaav.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2sqkuxzbn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2bjjxzoxu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2jlwpzfwm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2vmesbrwy.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2gjouyrta.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2cagrunhz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sgzititf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afiyqrju.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2efdyjpoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bcnrtlem.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ohbqoupt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2qvglihvg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2thuajmvw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2fqjoyqcn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2pkvoskza.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2lbeuqovj.html


<!-- 参考信息 -->