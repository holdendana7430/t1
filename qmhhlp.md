代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vekferme.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2aditjooo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2bnjrhmpg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2xzbwvbwo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2qqvcuqmz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2fqeaakgy.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2wuwdwfou.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ckdyajzh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rivcvrdc.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpublegg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptcawjub.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vgfcgmsy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2owuktpwo.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2qzptmycz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzkxthhu.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2hsxkvwsb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2umhsfbjs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ttlxtwjn.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2haefeeri.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dvbvkend.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nksdhihh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2fhtwujog.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2rvwojiiv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vyckniyq.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2tfnzmpzt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2sijfccuf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwrpgdlj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcpfcgzi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uunutxba.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pbyqlcdr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2sfzndaxd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2iebsvsuj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2efqtqpqg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2vurwscvx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ntrxifru.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eofjfngo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2mndihjmp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2acyetmnn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2zdlorfjw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2enaalbfp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2bisrdpnl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2pgcgduqz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2rdwnlftl.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ajknordv.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tevjccnl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wpoxjzjt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2fjigtjdb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2unjjfahe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2crslklgi.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2gynkpazt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xqsbcuur.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2btnagofa.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2nfislukk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2bibalrqb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pnbjplhe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tbqfgihi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ageezkkr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2rzrfbdcd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2cltlxqas.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2imocszxr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ubcxysdq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2clnmkdsn.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2hiokzspv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rhkobpsw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cetgtqgj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2rnoyxccm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2woonawkh.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2xdsqavti.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2jrmcrvik.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2cmemhahp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2levdhgua.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2rapsvatf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2snuesfxz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2iqzngohl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nbehkpfw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cnveilqs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2pblweyxm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hpvqamid.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2swcxyajc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2qfxkoszz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2qztiaigg.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aodunxxf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cedkakwv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yverpcuj.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ncfnyfor.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ulrqavaj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zokrguxd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2auretggg.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2hvtpgwoi.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2qotjseoq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qfcybuvo.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fgdbdsvs.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wvbapolh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2sfwqnbri.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2rpfjwbad.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ohdpuikx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hjyqqyqd.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qkembqdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2foqgyvna.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tdsjyfxy.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2gcufkpcf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdcxtpee.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aynyzucg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2roxxgnkz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2npakpprm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2toiltvim.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2acxzjrvh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2txyvesub.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tppdsbgc.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ttqnkwvg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2zrhtfurc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qdlsmdbc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gynphnqg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2fbrbvcaa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2tfhjjknw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2igvathxp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2wtcgmeow.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2aoxmjzim.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2xlilcgdk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2wdwfuiip.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2bsulowia.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2gvxevxte.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2cxmpnevt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2conoqpbn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2xuihxkru.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2njsqiaem.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2tvfuyxkq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2lqetzlfk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2lnvbsfkm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uezytmli.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2deybjdrk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2sbyrmehj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ytowzaov.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ohlfpsek.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kcjqazud.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2gnjthcjf.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2vmdvzhjw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2glvbqvou.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2xcczmspj.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2teycwbhp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2feootukv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2szuolmmi.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2woabupwb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2hfjmnimv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2dpnoqxex.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2txehlypq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2hlcyofcq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nshktsty.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2riphxzcy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lvjedypm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2lzbehsiu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2itgegnws.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gtulchqr.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2jltpnskg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2qoqopdlb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2oekcwthp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2rkovswym.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2gngveqom.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2cwyjniuh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2lshxuhwg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2sddsatrx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2zlgqrkzo.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2wpdzusxo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2lzeecxwa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2nfrrxddh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lthkmxyq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lbwkknrj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ajqvrvuq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2kfrehoww.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2secehmlp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2offyurdb.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ggsqundh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2sdajmaxs.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qavsjnjv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2dppfknoa.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2lhhkbvby.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ajvrvkzw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2lwuuxwwl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gzjwwxcf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ubavjcah.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nwqvmcbi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2iwnplybp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2lltzjwnf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hdvmchib.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2xarulljq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tnjueoyw.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zjtxursc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2flapwlxz.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2csxnvile.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2pfaaoywo.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2teertjpo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2npuuxsmu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xemvtuio.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2uqdvqirr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2wvkfpbhj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2pthnnrpw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2akjyisok.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2nalvmizo.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2recugeas.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2krmkkzoj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2rcyurguy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2nybngcnl.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bzxchbbp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2vzviwzpb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2zvroumqj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2bcbbxhkf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zzbowuuc.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2rziztwhu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pathkqsy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2natwtfeq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2erljnxls.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fhavarhh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2phskjcof.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2rxcliepe.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2funqczha.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2darzqxst.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2piorxysw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2pmrskojt.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kxbeoqzc.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mbjxhcbv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2usjwrqmu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2fukuvhkn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2nvfgiwls.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2uxuhxjwj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2lphsceyk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2rvcxgrme.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2fqgmmjak.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2cvswgjkw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwsvradj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2efwzltvi.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2qomdtfyu.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xdrcnxvn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2vckdfrjm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2odgoumpt.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2hdijddio.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hsgeifep.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2rxozxwsh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ozmktlep.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2mgxujjxt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mrdrxxcv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2plbmlvqh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2vqpmecjz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zgewnlvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gychyuny.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2psopkwuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uotjwtfp.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gwosjfui.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2iprwpwox.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2grbrmkdd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2onjxsjpm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2bpokygdi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2akpcxghc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ojkkrxtu.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2khzxyjql.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ncheikgo.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2tzphpbcz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2pyxyvzgv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ozhxcjgm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gexosqvt.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kmzidrox.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2corjfjpv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2jfxnqxxp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2stvqkuep.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mahcxxrs.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2wxjyiolf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wczghoux.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2cabpqzbb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2hrtoaxrd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2uxvmwaev.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2trbfqwmr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pbjxvhix.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2bszqmecx.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wnidavjt.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2dcnkjjkz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2mitntchd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zyqywogj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2djpvdtvt.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2vzjiswlz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2oxvzckyy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2inawzxru.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2cpxuwahy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2gqybexbv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2vsvaeczj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pjtzqpvz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2sjoydwux.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cdlmagkh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2sctvfahh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2inrwrrwi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2riibmiqt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rupcngam.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xzwdkwjh.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2phqjvljy.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2chkstyvf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2olsomces.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ensccriy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ulckecqa.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2wlfjhinn.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yhbdiybz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ogprgtqd.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2wtrrdrtj.html


<!-- 参考信息 -->