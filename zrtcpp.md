代发 wailian999

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2afuihxga.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2fneempfl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2muejoxan.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2zvjolnjq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2gghtyhqk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2gevgaeon.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2umjuxmlq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofsrfhir.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dcbxzgji.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2dlfivjgg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljyjsfsd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ipqiqqgd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2qwzptvqe.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwqrlwmp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ecgdisya.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2rwvucyqd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2oyhlajnc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2hkrlxiio.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2afcabrvs.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzzzmaxn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2tnabklqu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2emyaosow.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xcvahhsw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2lbhzddrk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2bcqaoeeg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2sdzqkcly.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2vwwvdozg.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wnrwrjti.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2lfgrhtis.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2eayphzbg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvnqlrvv.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2snzgyski.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2nekkdtgh.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2zmkmprjt.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hluhzdsl.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2hmqaqerf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2zvvdfmld.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cahlrbgd.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xoetdtiu.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nqrnlgbk.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mdphprjm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2fqgbkgyv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2dfiwlreq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mhbrfqmw.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2pltawshi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2cereajxr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcchmulc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2elrluewd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwbnboef.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2obkzpfub.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2khfyvruh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2arhtwing.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2frvdajuy.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2wmiscewu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2cbavkenj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2mmkgpzvb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dekyzggo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ickqnsgf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2wpudntoz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2tkfjtgyh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2nnzuupin.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2chorwcnl.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2gdubsgbs.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2pvqrammx.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ufkkubxc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oafmfwmz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2yfgxxowo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2vufqgfjl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2sobmbccs.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2mvrdzrko.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bgsusnzl.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2aesitrji.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2vsrgpyms.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2yhtaaxqs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jsqlroep.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vmvdwpja.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oycjcvrn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2xsqitsdh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2fgztuxvk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ysdjhiox.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2dnyonmqn.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2vkpxiaaz.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2hthhobws.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2alvjstha.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pmmosjye.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2uqcykmpe.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2tvincinu.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2brnfbcqr.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2qrbnvpez.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ptvutauq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ucixzegq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2zkpsbncf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uqnmnxda.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zvdcwddu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zwnhubum.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bieuhbgs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mxumvygq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xfzroyet.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2cntvecgr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2poexmkpc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2vebokcjj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ohezzjhj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2amciqcrf.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hsepuqpf.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jyuoqujq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xstrlnhs.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qoxmkjnq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2zoiyhwpe.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2qsfkubyf.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2lgdmmvnw.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uembcngt.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2iultcvue.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2qkeysghg.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2hheodaig.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2unylsxyd.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ukrevxsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kdqdiklm.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2yeavibrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fdobhbrn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tymqnukk.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2ipmzniko.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlzqefnx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjsqmwry.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vagdplcw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tanstsoe.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kpvfuugo.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2yaccvryu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bvmoqtwg.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2bvvzbaij.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2rhgerpkn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmahiosy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjnyfjxr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2boohjjhj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2cyrarmiz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2hroeqben.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2qpqrnbgj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2hdmcomdt.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2qqvplmsm.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2uzfegybh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2pghnoyoi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2slzrelxr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2vxmeowck.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2bzrwtgvh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2kmiyttsf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2wpsisuef.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2rpnagiyf.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2zxttsnks.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2watftirb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xgrctkvl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2inmboltz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ubmsttmh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ogjbhbsj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2knhmqelq.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fwzdqqim.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qrotcmnc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2rgopinri.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2blrmvfoa.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2uprlmfdg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2awavutet.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wxhxdzjs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2fzxckexr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ptjzyzmt.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2carodkmd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2smfxbnvn.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2piyhonwm.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ypjiiufk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2bmtpqinm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gnibfove.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2einiutgk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tymudnrs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ktjowdbu.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2udzmnkby.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ncvtwykb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2rjrlhiie.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2odwlsidi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2cinpthvs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2nogovfgo.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2rvkmadne.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2biwsmxoi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2vgpbdken.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ifdnqggc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2mngmftjg.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vlknjzdc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2honpmwro.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2fmfqoqgw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpodvdrb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzcremcb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2pyylxlju.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2yyfamatg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2jcsegwvh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2igrnrfdg.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2eolggzfd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vposlkri.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2asuozjnb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2wajnafbo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2gazqvcye.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2fnhbeqyh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2scaileym.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aguwiabi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tzjofgsh.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sspbkjfd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2kwsjokze.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2uriiybag.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ffziuqmx.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fvqihrlj.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mwjzanzm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qqztsefq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2mjuyqzqt.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ouqvpgqq.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2vstfnwzv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2milkewnv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2uxtlhnyy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qwpppglf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2bklwinyz.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2jyutanqe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2qmcugooy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2eiknrmbo.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2hzfqmkjp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2rflwiozm.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2jqslvgqa.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2zkdvbxxy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2nsahsbpr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2wxnncxxi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2yfqtwywm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ilrcthbh.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2iviwlzrw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2mxshpita.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2zhacrtli.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lnfurqcl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnrtptmv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2okvumkfe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zektmpjs.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jmdndjfn.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2mbnxuemj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2gghtmyuf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2krhmzell.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2xljxwgle.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2fbttpcix.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2okzdfxfq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wvixlmyq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2hbstlprl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2vfnpcbvd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ssolaxbh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nxaxsguh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2jmlwrluc.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ldvjutjd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2xyqxggsq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kyihofpy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfrddqke.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2mkbqmlcj.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2lfmflvez.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2jyatrrfa.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2lpkqmesc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rzjighkw.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2zuzybuge.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2cpvosyii.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2vjsstwhv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2asxqkpzf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2mknndhll.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lpvdgauj.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2bjghjkzo.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ycuzkpkm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eiuwepwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2azqpqruy.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2dctpjnre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fsqcefdf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yxhybcqg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2vkttgtih.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ugnrrvjf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gjbakhgl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2wsihnvrt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2hbgemxxh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2lhcmtjhb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2hkycohpp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2mljhacuv.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2azbqkdwm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2xpauaqrd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ibbjzjoz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fcpnqtnh.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2omwmroox.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tzjjycro.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bbfatibi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2gagovtlf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2taxdwqzr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2bpkphokq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2buzwrurl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2utyjcqbd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2hrbcqcue.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cgnlcmcp.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zodubkoa.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2zyengxzy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2cfpjzirc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vizdvevt.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ouhghlpk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ofuijnnb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2oyrtbswu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2licjmwsu.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2eapduvpy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2redeltex.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2tmvohplh.html


<!-- 参考信息 -->