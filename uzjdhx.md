代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ujixicmp.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2vxvllabp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2sxbqqtse.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2nsaptats.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hkwoidmy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2porocjbh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cfzzqagz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2swcocixq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2fiiqyzri.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cpvsvhvk.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2lvckmmkf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2vuqltgow.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcgrakny.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nssmndee.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kyhrzymc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wstkxuui.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2hhrcchoh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2qblsjosf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vayetfyf.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2gfaawraa.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ovbrarqn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsntpsyw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2eyzsmtqs.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2qdoyyoen.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2tefsehia.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ytxrasdi.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ynrlbqpb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqvlxjpr.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2apdjcqln.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2tzhiorkp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2jjptcoll.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfrhdwmg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xxivgkhp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2katvnyol.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2lfbnukaa.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2tcqyxiqz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwqrtxfi.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2utfrutbs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2jqhbangl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjlfdidg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jzyxwbml.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2mpzuwelc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2kamqmqwj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2pjzpxrmn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2dwduagxb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2lbddtnuq.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ikmnsfku.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2kynuprld.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjralcxn.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzdstzwu.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fchzgntt.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wxlnayfq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2duuomnms.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2tabggoel.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cjlgqbez.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2srsyrcqp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2opqbdkdf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zfvrjphr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2spamtrhw.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2drllawsb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zslfhofi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2hvjjxeyq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2xqayaplt.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yidgojkm.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2korzdtnh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2xwblorzc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyaspsxt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ruzfsvsx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gywckhpk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2luejoedt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vpzlpito.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ldaunswh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkirmsqf.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2cehleanh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2hxprrabi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqaxgath.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2nxggyqrj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ucatjvfw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2wiepwokr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ocjzcwza.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2rdrekquy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2vjcnesal.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2atmctqgw.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2yuhrahfg.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qyxecrbe.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2egnttvop.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cngncnds.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2nlmhmsgr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ivnzjlqz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jpnryhua.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2olwumwbe.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2lgpmgpso.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2zbxrdbqc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2leevajai.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2btatnogu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dzwosdll.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bsxnfwib.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2lemacywj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2xijurnsq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2fgzzbuhg.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2gmmqhbii.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2kovnjsmr.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2mfkzvzup.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xalphpaj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gxmebwad.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2qewlnfdk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2xhytvqyx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2vtrjtshr.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ticognec.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2lltopcue.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ilhdicog.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2uuyycfrm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bpdckpan.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vkghscwh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2efphfast.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2phiefldb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vpbxslcw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lbvvyixb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ojvdkbpc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2jmndmkbv.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2aryrhjnu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tzeylqnp.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wrccvmpj.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lajenuxe.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ablrrkak.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2suymigbs.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2glpzwybh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wccywwyn.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2akvkhvlh.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbqbxhaz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2irogndac.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mzekqyar.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gzoxxvat.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2rhzjskiw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2xquqmahk.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cpouflql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wsvnxeyy.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2hfuiabch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vzomchjw.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hgwdbzin.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2wwislqfy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wgacagmf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wextifsv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ommiebfk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xqsvnexs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2eujfeopd.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2aacqxuhd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvakooln.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2udefsukk.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2illbqkqp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2wvoanpyu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwczpboe.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fardeyqy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2auuzrktd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2rxehxwzs.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2klnhrqeu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2awktdvpr.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2ixaldtdn.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2znnogasz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2cqcqkwqh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lqmlblzj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pyfsolqb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydsiafcw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2nazsbkre.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2mqrnnupf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2egteokcl.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2phxoqooj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2migpeduq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2tinoqabq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dotqrwxw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2symobypn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2hsldflaf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2vdypbzmf.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qwovenhg.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lmhbnvae.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2nlxjahaw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2pwjhstxq.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2damgzase.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ngxgnmmo.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2lqgvujfa.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2qgbjjhuz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2yywtanry.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qunhzphy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2vatifiov.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2dytvtjvc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2kfkemopr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ntyfopem.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ukgszfsw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dyhttovg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lbsutkvu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xdyvbofu.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zdfzonsd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pbxhzwfx.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2kgircuof.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2lqqxdurw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bjdhjxmx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2zuannsya.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2xqeakygb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yksteemm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2vojsagdm.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2wsevngko.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2kgluwauw.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2xxedbdtk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2vvfruevv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2vrubpodg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2atwljuvi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2myvalyjl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2eyddtbxo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2apnioswb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2loivalnc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkbpfgsw.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2llmqznuq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rwwkqpol.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2fmvwbzes.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2dcmldquc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2uejlcioq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qkepgybb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2lebpabai.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hksvurre.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jzvbiyzm.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2mcxrodxp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2hbvhgomi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2gvkixibc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bpeddlqx.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2fawitsov.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jsizpyfp.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fhmcktox.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2hjzzljus.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fompggtq.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2brhwcseh.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2iylsouhs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ujuxmdve.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2zgmzzytl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2dktixsst.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2wncgzzhe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2jggrmcjw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2eqelossx.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2sweaucyr.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2pfnlasxc.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2vyzegiqa.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2hqmhhtgi.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vsofwifd.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hathyzux.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ukpagcve.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2kcxxyczo.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2vcfgngoo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2boeilynm.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ewdzthta.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2gbmkmddi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbibdfgy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2bvtunpxj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zgdsogby.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2miewzhtk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ydpzunhq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2sqreiigd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ovrzpcno.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2lmjkevon.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2zoflubuz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hiugjama.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2sgmnyqoc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydzmfsxo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rtqgbjfj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2mthiwxxw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rqkuparw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2uqevbgan.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2qctsjjgv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2aodqlyad.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2usbfsffa.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2eunlfcse.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2kvbalgtn.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ruzndgqo.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hnqvfyse.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2okacsttr.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ffqzymec.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2xdznasfk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2kdxfnrgq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2jxfjhobt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2kksrczgi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2hyfkvctp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2qlqjlagd.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2fgtiaiyf.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2fckjjdrv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qzddrjot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qesupcqa.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2kzpmycyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tweieefh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2odiqsody.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2rhscekbn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2vjepsppk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2vbeqxqfu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2pwxmpeev.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2vpyuctht.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2xncqzcuf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2khtphxhe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2nvzhoaev.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2mzllglyj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2lxelgnru.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2vayygluo.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uzdzpwfr.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zhirczeq.html


<!-- 参考信息 -->