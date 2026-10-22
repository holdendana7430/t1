代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2wrsfwdjr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2hyqycpxp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2dliptyuf.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zmcyalar.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2vkqkxhrj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2obycmvji.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ecbxlmub.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfryydui.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2tgjxbgkb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2cnwjzthi.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2yatczkwv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2melqvbyq.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2nurhjpjv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2lzwnngjb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2pvgzgrau.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2wlqsrjgj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2spwtfilp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2qltkklpy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2nsfduolm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2qpopxebu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqrcdxhn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2pdsvvufk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2jgacnzeb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2cvqpvsex.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2cdmuaryi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2tjjqydry.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2dmfqwelm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2sohgnyqk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wvuleyxe.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2lrajwkgv.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2mrwvfesf.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2teljvscl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nerrzvem.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ajkvgzbw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2sxvqquqx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cvfpydax.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2snozecie.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2scdowzry.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbjiiybp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2supuundk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2qjxvbyns.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jieficqj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2khrgxexv.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2finzdiwh.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fpsrxmrl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2mqxadrce.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2cfyazolb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bditpxwd.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2wxuvrgvp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2sclfbbev.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ustrgdht.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2duzfajgq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlrnzpah.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2iaypohvj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2zuevhtmt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2qhwzntde.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjlclxzs.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2cwjaycqv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2heegdqww.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2wdsgucvs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2jqgbqlex.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2uqjmlksm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzrvdrdv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2yxyrxfqw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ibxavsgu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qbrkgtdi.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2qcgoqgzt.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2txzhfziw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2noddptxr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vtokalpm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ejrzsvsz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2awztohkd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2bfiwgakr.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2uklxttap.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2msbhubkt.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jilahboy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2fwrjtvkp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2qtwuvcip.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2efobglgn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2temxcmqg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ecjpemic.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2sfeckwui.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ovgqecps.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2pfrsfuzh.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2wiafzmwq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2qtrzeyyx.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2adanjlrd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2kjbxwmed.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ydyggnhl.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2vehrwhza.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2vaeoujjz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2pleexlvz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2srflaxpa.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2txezwled.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ptqiuugr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2gafhkuyj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2reiywtff.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jkokxgcd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vlkskcki.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kfwfpgmt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nlzofltz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rszlrdqq.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2yjgjdrva.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2hfeuiqur.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2scyroqsz.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2evgodvqy.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vcaxtlwu.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mvnnjrol.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gmuouuos.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lcaqfhrv.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nnolzybo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2nvuupiln.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2qyiabtih.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2xwlrkmfg.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xwofhvfx.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ihjgamvc.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2kunldjoo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2aduydntg.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2jioarhbk.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tlefkjnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2erkxlhdl.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2yseeqlgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zttvalyy.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2zggcdgso.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2wbmxnxtd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgllbzrs.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ehrxezrt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwtrvfpx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eulmedhl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dakgmnta.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2gncimxji.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dfxzcded.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ugnosbha.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2nsduoejf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2yceswtrk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2scrjfhjd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ssbkbjaa.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2byieclnt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2onibfled.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2emsgqxbq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2brjyygme.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2sdfobhjy.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ctmyxnwc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2dhffrwwk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdeaoehe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2npsajggc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2funbvcfo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2wdjbeirw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2amarowsd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2rthudybz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2jwnywifn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2eqlbecnr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xkxarzco.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ckzsxtqu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hdkivpzd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2vbrcndqu.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2mrohmfvh.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uwarhdyq.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ybscuwbf.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ajtqgtqb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xutymvnm.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2kmlzjume.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ytqhekda.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2yyqbadzh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ippngcjy.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ikydayzy.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2dccmuimu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2qepnztti.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2kaitzrhb.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2icxnceir.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2dnbgisec.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gswlqyqt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2iikbdesq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2uaoacfgo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nwmubxcc.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2igdgkawd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vrdqgwzj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2jjlvzeyg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2boeezcde.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ztwgnchg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2lelsckxu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2eonaziyu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2aqwkmepo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2lbswgezo.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2hqobradv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2wxmoxkvi.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jgteqklq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2dtmmoxuh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2akdjplmz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2usrhgvhs.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfxsjfvo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2dpnfobee.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2tqqsrbrk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2gwkujohy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gpsgrrqk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2hbsgdwro.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2muimlcmg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2olgxqkcg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2foduodoe.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pbwtoejw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qeyncmxb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2thninriu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mjmtkmuc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pwwebumj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2nolidvzp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2lcvjdjaa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2lsgugwxm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2aoddxvhn.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kofjgigm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uqnvhyon.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dlnzqbpv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2fuzcyeje.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2tozyarcc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2igfjuuvc.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ahjujpbr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2nvvotqyd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2gdgooznp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ckfztmjt.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2uuiwziju.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ojzxakyd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2updqkgfb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2gzjloqou.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2cmhancav.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2oetsdyxo.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2krszmnfj.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ehvdplwk.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2smwmevpo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2crkswbsf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2fbugweko.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2zzsxvbeu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mxjrhebc.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2rygmfzuq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kqppyufy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtnchnfp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2fvqbsbjj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfxvtmpe.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rfimhvko.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2vhvxbqsh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2dflmaurx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2gazmqkdx.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2tngwccwi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2abimznbo.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zojxmxjk.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bxrnpyjy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2smxhrksz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2gsofoehj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2uecosavt.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zubjswzr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2dzjvomxr.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2blsvhuac.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2qhdekmuo.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2oapcfgjb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2tedglpwj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nrbmskxj.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2nnfyxfsb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2sfotaayn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2vqffqxtj.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jogptvna.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2qzadppfy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zzovrtpz.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2jxorgxfw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2atkllrme.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ncpkymlh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2afsjjbkz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2jellqpup.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2uqktydbm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2xmdjqcxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2julkltdz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2kvqpqana.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dydocxba.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ihvegbqj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2swohidrm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ebtjqahh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2iagtbekg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2gcarwltn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ycfdngko.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2mvbiqsqn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2qkaldakk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2xhdfjlgd.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2vvivvwas.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2njxastjm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2qxkyvgjw.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2rwplhnhk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fchvgbap.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2sknizvzk.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ddeuwszb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2rsmawqyn.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2oqfqqqzz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ppweupdd.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hjupsgsd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2oplwohnu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2fgasjktc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uapaivgy.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vlbrubpz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2dogwcmxd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2girujdcw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xhpkoaqj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2tsnovzzv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lyxyrptp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2swjolngr.html


<!-- 参考信息 -->