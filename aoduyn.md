代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2nhboaziq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jktlsazm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2nyvpruek.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2cwwakxvd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2grenpndx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2slxefyhh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xymautpm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hypfbyel.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lileobns.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2hftnjztt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2kcsnxwxi.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2kvkzsttq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2idsfhmku.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2axezwjbm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2bzlghbbh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2iyxwtsor.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2vwtuhmgn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2rnfbsxfc.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2aaaqoipt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ngvhbfko.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2snzufxpq.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2svilkxwt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2dkkpvioj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcuxeauy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ybxwhpvm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2oycnpatz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2dcnyqfak.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2wfwqgkrn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2btstypda.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2htiotwjy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2lnqwwffe.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2hiwzvyod.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2rvkpuage.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xujhnoym.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2sipwmgix.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2cemcbadh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2fdneigzw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ersjfyfp.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2wcrubgne.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ormtehyb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2emtwjlft.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbxkdyab.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nhigekpn.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fdigilaz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2bvisozlk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2dixnzaxy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bytbzyuk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2axmcslcf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2jfvzklpi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dunkzopu.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vhohumke.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bmusmubb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ajlbhwfe.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qjhwuphr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2zcdrfawf.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dibezjcz.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2hyxgjvja.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2djqvvays.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bbfoxkwh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ljmkzacp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsklyunn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rjakkupi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2cvedwdzg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2irzbybzo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvuieccp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ycfgjfao.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2qoocuxce.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gflltfdt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2wmjracke.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2eznaxbge.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2zlskjjis.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2lkstgsmf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2rgldjgtj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwymrljm.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2jvpdosul.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2oufzanjm.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qaevbecd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xrivqeuw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xgtmhsgn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2aswtfqcl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2vmvkefve.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2uavcxkkt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2walekfpf.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2tmxlkpbs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ecglhswb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2mdldaiph.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bozdkxlh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gcktjqvg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ehhzoqiz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2pmlbhzyd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2rlcpatsc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2vyigpcua.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2kurijndj.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2omyjrsfu.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2rtggpjte.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2umskyjhn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zhkmarsx.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2kgmlrsbo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2xhvzszmf.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2yztfbjmw.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ncmhqify.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2kjguprvy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2avlwcysm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2mmiefktb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wtqzulvk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aokfmnkj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2izdjktog.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2toxmivmy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qzaavcac.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eppwsqxc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2xalfaarw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2jqnyoudg.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2ehmyvluo.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vhvniitg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yatbfcvn.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yfcaybml.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cgdgqjbr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2citxcqhl.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xiiwjzdr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2msrwhdku.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2lykvyqrg.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqenhshx.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hycjkxzh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uztenifs.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tpxbyqah.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2izsygmga.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2sqqcxuqo.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zodptsuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vspwbbig.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zaqddzbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tkkoynon.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2uuckqmin.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2gituzevz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zmcwegfk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ijvrugzd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qjytuadp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2etllumdr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2icdhgxul.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2vqzjspka.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnpajbdg.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2pzcjibtt.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2xsglktob.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2pspoldug.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2twrwasot.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ibntsblo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2cxftjvys.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2myjidpat.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2wfddwtyu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2lnaijhpt.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2dibfvfdb.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ktdtzhil.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2jmcsrisb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2dcawoenu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2akognfnl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2gazhxjxw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ayropllr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ybsynzum.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2dcnsvcrd.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2qikinkzf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2wtmiwoqm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2apepewve.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2jqgrdavr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2erfepgdm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2yfbihpmz.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2oudicwfa.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cbymejue.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ryeaiucg.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2cbwdboop.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cowpyjwh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2fofmvion.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ijwrapyt.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2jpdwhauq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2hcexxnfq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qpbhbecl.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qhidfmyp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2fdsnfyxj.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2bhsrxcfz.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2omfjhlvr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2nsnearqo.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2odgqdfbn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2fuzgvewr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2wssmzqfa.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2mpnhfkyf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qnovvonk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ynfokzjj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2csbandyq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2bdpojvla.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fskpxadk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2pawbvwiv.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2bbznbtqs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2diydsqca.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ebowgahj.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2tcqhsijz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2urgrntbm.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ztkmrfrq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2lrghysyh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2jfjymatx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2cgefkzuc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhorvomo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2zyuhxbof.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2atxaealz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2mndtumtf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pflcaxte.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2envudpao.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2byypqipa.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mjhhykst.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qczhfdgn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ryvkuhcm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zvacvfwg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2hnukojvm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2pknfmdoj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2hugixgih.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2eqbvuksy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2obimhsox.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2dxkljsxb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2jvvacjhc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gfashiki.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ozlsiavx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dkmkyozr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2nmdkcumn.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2iwhdoaax.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2sjdqknaw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2bqznifln.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2dtfvlymz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ezdnjuyu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2adacftoe.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2lqivixcd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2kzswyisk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2notzeeqi.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2gsjeiptn.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ioquufdj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2zqcvkilu.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2nmvsrbnf.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hkqwzgiy.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2mweajkka.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2vbxyddpv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2zmremzps.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2miwgpzjf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2celigsvw.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2sjiuejta.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ihiqsmne.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kmajifmh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2jsmlmyta.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ejrwfnxu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jrabcfzp.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2xeshllkn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ldivxzos.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2hidwwvhs.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ypmueynq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2xfcfxscn.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rhycaema.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kvxqvpxp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2rkmaykqs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ysqkczoq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2yxzrkuhp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2glnkgout.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2kzfexaar.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2wvzzkvlg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ftwgztxr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2iuymceoe.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2svtcduao.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmiutgod.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2lasovtxo.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2uoakpcwg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2yebszxsu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2alglcctw.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2bqyowknv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2nggoytle.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2hheibxrr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2msxzhopv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2fiufilps.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ogtmcdsm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2tfratufm.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2yqmvtras.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2keosxmyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mguqwjkg.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2llimirbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eoszdwky.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xbhuaynx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2lrthshqh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2awvthvtg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2qlfggdzp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2cetafwjx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ystdpltj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2hjgnjhnt.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2alxvuzwr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2eeuplgrb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2sqcytxpk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2oucxjgcm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2onrensxp.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jgzraogf.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xjbmmpgy.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ojxmonzl.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2jkcruksk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ybfltcvw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zdoxmcdm.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2lghymwtg.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jzmiqwzj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2enbgshpj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2cveuawgs.html


<!-- 参考信息 -->