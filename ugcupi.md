代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2tychrmjb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2hyifwvzn.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2nhhuxkyp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pwlmtzgx.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2eexkakdq.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2axhvoees.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2bqmbljza.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2cinrqcfu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2nseieqea.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqinpzje.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2erukieug.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2mxvtpnrn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wbqmokya.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2femazkme.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2suqgktdl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2wvruxhwn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qyuwfwmf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gzdqeppp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vynptlai.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2mdeujhav.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2jiegxret.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2qzqxbvxg.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2dlbggcmh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ikkxohxd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuyjwhts.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcgiwxow.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qakrmbqc.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdrbheoa.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2vkxrbtrh.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2nfsjmgrb.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zqyohojc.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ipdqwfqu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2eiyilnpa.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2iifdqdxg.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2byxfqfyn.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dpdzaoxa.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qpvkppqe.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jjnmfzcp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2liolghsu.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2swtvimqk.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2itzbyigb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2htxtiasz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2drilddrw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzwnmszg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fltmmrrx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dljbgjiu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ygcwfdxx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ylhjjidh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nmxngqaz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2zwlfxxii.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2phwuynrk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2hzdqoyzx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2rrozajpu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2rjdfzfru.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2eobbtjnl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2aaxkpabh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2rmbwszxk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2hikcbaww.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2xjqbjcbn.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2jwfstmhh.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yurpzcra.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2jcqqprht.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hrdfeumw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2xbysttsq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2shrmnsaw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2vvvrvgvd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2vsjgwrvx.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2obkuqfga.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2jehzxwnf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2odmqvfij.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ojvifxhs.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jjuuufbl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ajgnaiui.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2updbyspg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2oqnvwbqx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2tsgyhzmq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2eckthqsu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2cvaqwxbx.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2tguvsazj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bpqrgazb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wxmvdisu.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2czwqvksd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2asmlramp.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2aeefisuy.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2krketmod.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2nbpjoqqc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2zkhvczao.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2htidxhhg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2khkqvyky.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bnjhqbfc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ihjxtngm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kcyutibr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ifkhmytm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kmphqyzm.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2azlkejhu.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ppxqzqjm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2svodaszl.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2iuqwhmnw.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vrrgfhnn.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2omfvzpjp.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lzfeaamz.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wepnjgzs.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ltsjwkzw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2stzslxce.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2jhkwhtfs.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytxhipqe.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2grrmryxh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2asxgrbwz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2onuaihww.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2cixsgkwy.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2qmlawkvv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2lbcqncti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2adgylmou.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hvzjcwke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ledxfahw.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2buksdkcw.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gcmyanpw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ohhulnui.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpautgzx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xaztuuyz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2onshcaqg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2wlvyeyfv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2gghfkwdn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovmjrtho.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2amaogbks.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2wwdgswgx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jyxyynla.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uncjedzq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bscferan.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ureqjxlb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2xbbvpaih.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2wtfdedvn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2fcdawfcb.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2uplmfaei.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2hzdrgovd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2asmbymkw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2gztkfbix.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2crveetcc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rcosbiim.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2chkgsbbq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2uuyojrja.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2tynsjlfd.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ixhckxqw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2mdlowpfp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2egvmowyl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvnidlqh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2vsdknevv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2cluwmpjx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2tzbbslmb.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cfrhedti.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2atyxdhlo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2bwohdmrq.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2befyvfiq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2rrwjcjyw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2hyzinzhm.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ooeazxdb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ylowwgbn.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dgogjxiv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2uosyfvbw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2waqvpmnc.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2bxqsrxrv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2zeglhnfw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2xfdoiodw.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fadkgcxi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2stgyzvuh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lcdotkir.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ptznyanb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2xrkwswrv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wsnoimns.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2dxjoeohw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2kwvytlhd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2kulfdzov.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2legftunq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2enxvilst.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2fmawvdgs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2qsxrgswh.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2hygkpthv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2qhnvxlxo.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2kbuzarfr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2czndjnxz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcmnlpgs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tpkwbeck.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2afxdlhev.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2gtrqjpof.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2nlkavdok.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2qgmogzgu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xlhwyntt.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2acyuzkdc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wadmyicb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2srjjeuyi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2tucystka.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mimpjdao.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dlevdoem.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2gigezdlm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2tgqwbwya.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2uaezwoiw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ckljeage.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2zkiffdac.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2eaiirfcx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2qmikkown.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2gohknkmb.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2eqhpiijw.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vjypxcfi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2jvozwhcl.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rrpxjlzk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2paqvcgsl.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2zwwazjhl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2kwalbomy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2budvbvwz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2qrogcckr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2vcpbfjys.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2sskaqzsa.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ycmrutzr.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2pctotyma.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2dooqjtef.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2rskywoiw.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2atmjblfj.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2spedfpei.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2qtrildtu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2emoqenhg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2wmxbtgmk.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2yfmjkvxl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2nfahvxai.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ltwskwly.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2dllvuwlm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzaguwim.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2epjljymr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zkxieukn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzkzaiwr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2gndhbofz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2tlnksaue.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2wfeifbyn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2klldwjgn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2omhgiuan.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ztnwcmxd.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ijjraexy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2svmnvkxm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2iwzktgnl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2nprrtkol.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vfeqwbfw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2lojmbfuw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2zmvbqrxn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2dfcmllhl.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2uksdmnwe.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jiedbfqh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kzhhdxig.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qhpnzblk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2dyhlgyne.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2avkyoilt.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2eztrpwsz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2udkslwth.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ixelryfk.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2rcidcgxv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2olocdmvf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2azyaepyo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2xxjyxgph.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2nvyosmck.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2xpkzgpxb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2idldqlro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2btctnvjv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2tejiubbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cdnvisnq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2pmhqsaev.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2vcqcdade.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2osyfqqak.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2iwbwldas.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2zfqluqhx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2mjmabkha.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2stmgbldg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ovlzbvla.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2zcivwpcs.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2zaupsobi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2qjiehmml.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2mvgvdwcv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2njueiocr.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hlgbkhan.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2qdzpqjhg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ejctjkgr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2tpptqhhu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2jelckmej.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xpdzkhaa.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zqxlddcm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2aznmgrjy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2lyyoqxbt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cigwwvix.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kdvrmwab.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2qoqagqew.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2idcnoowt.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ajvbcjhp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2oiugsrei.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2dpwhncku.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ejyrljpj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2fjtircuq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2egbavscj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cunrgpfk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2porraqmu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2scyfruhh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2xiimwakj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2lppfoytf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2otvbrbem.html


<!-- 参考信息 -->