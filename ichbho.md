代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jekkkwho.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2bkczyzbc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2yqkelotd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2gxlzoqag.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2jbwuhpyj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2pkrshaox.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2hninwomi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2rpvvndpr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2rsjuguhh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2pzeqhxlj.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2bvlvwhge.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2vviiovlc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2eszqnwyj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2liiqhqpw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2efnitsyq.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2punsdowp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2fnhsaopa.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2dlkpllif.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjssnguc.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2kbokhcio.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ziyrzskg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iqedgjif.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ebgvjttu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bstlrjem.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wezdrsgl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2pxzcikrr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2nbfaqine.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lgfkjuva.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2bhipllxj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2qcdjharr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xozedogb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yjxrdspe.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2enaofzbt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nzezegkl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2mmjpfoco.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2xdwvktxp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ziktuoxw.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2pcqookmf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2nnttxwfm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvqkclnu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2aazbtnrc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2suipzqbs.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2mrijakkq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2tyhwryhc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2dwjsyphy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2sdvmyqoj.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2wqpsagof.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2otoumitf.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ujhwtdsg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gdcsumha.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2rcvxnmil.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lztdxngc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2rkxovffh.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vysverwu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aidlstlq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2bivfaphb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2zyqsccrp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2hgiaevjr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2abzxbvfq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rdspzdoj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fpazplxj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2edrkedfy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2eczawvnw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2irzrcelf.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2qgwbpnhv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2wrpekvva.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2iuymdpxs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wmiahljg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cbszoext.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2hdqzhuet.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2kulrmpjx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2mpklndsl.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ejungcwk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2bvdlxfdv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2izygauep.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2sbssgdde.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qqylsgqi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jbnodtzh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cnabtyny.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2snwkneff.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qdnkihmw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ljvzhion.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2tyqyncye.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2fhtagoyy.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2wvorrtkm.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oiecrkfh.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wyrpstbm.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dltbrasl.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zvylnhgb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lwownmsg.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rskcfyhp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2atjqgscm.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2vwzgdcnc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2sycjcwbg.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jnuzknpx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rrlmndle.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jtbbmyrm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2nxjosngj.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ueafjqpr.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yrtnqwjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rcijtqaw.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wlzpjwge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bqqxcbkq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2grigrops.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2sedhceyy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jzatugbq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ntneeomi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bacshlrt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uejleicj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2yrgawhfa.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2muzakffv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ufbfrtbb.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2twcnwrjc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2khevhuqg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvejyipz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nnzjxfch.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqghetys.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2khdulcoo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2jchbctql.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2kpdosoov.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2kxjntvtf.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2lkzlzcdc.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2fpvlssge.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2rmarqipg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2gyeyulcj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2swnrdxpu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fjasdyts.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2fzbojlfg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2rczhvlxk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ptsumzgs.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2xulmdgdu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2awjwcose.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ehzctdsj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2zivpsjid.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2hfchunpn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2uhvrgryy.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2uqnmyunq.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2blclnocm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yykpgtnq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2kqmmmnil.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ntznbswn.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2iaouhlrg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2lppppkrt.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qydvbodz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2katuqwli.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2tgpcnguy.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ezjtcpvm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ufobrbwx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jzgfbqnv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2oeeosjdu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2absueakr.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dpitaaot.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jszlchaw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2liopmrsn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2runbcyqs.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2jmeolvrh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pdmditdm.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2jxseyaou.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2visddvvn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ghoddiod.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2urmaxdyq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2xeydeecv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2idpdkxoz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2oznwnxjt.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2tpmzndsm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2kjavqebv.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2yaivbvrf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ojaaxhos.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymtcuoia.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2oqltptog.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzrxwwnw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2wsjeqxvq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2dijhevvv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2hsmpovim.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypfalobt.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2vaffkjtl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mqcmaijx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2dfscdolc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2tezffhkp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2sfiivfzo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2sboznmek.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2qetnbbou.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2fluisldp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hqihfvgr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2vciaeysw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2xpzakboj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2faloqbrk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ekrpwmii.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vdavnewb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fgiaukec.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hcdcyowz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2atgddnhg.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kxfxfzxb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2oqauxwfz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2stlqxupu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2iflemfbk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2yhhexqsp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2bvxzukux.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2mjcuizba.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2edzpzxtv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2gpkwkavh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2lckckrjp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2squtnopc.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2bhlsnjwd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2gebzafvk.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2urpjbune.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2dbrthscn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2vbrygasv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2zqioaflq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2wzhdqvbf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2orfqlqcy.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ruxbjkyv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ixymtqoe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zucveabl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2dnbwygsc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpuxhzel.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gssuiakj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2sqylscqg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2huoxqyfb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2qghqehhg.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2xmepktmd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2pmoallvr.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lrupkeoh.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ywrscxyd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdtioigx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2yesogfph.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2otvnqxoj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ytogsics.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ordbobra.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2thcddhsj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2psvjbsbd.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2yllibkfs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tllwtifx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2pxskfhns.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vztbnedj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2cmaxjbqo.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2mdmwwkwi.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2rxlhrsum.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2fjoborin.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ocvsagsc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2wkyebuwc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2jnyxbxuj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2kjjgmzot.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2aezvgimb.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2vfrxatvl.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2hahebfva.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2wucjiypq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xuwhtkxk.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2fghnvwbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cgeahope.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2yimxjglh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2fewejgrz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2etirumvf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2dqkegizh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2hqgqdfpm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2giccbqjm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2jzizfgdx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2qhmwafuc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2rjgvmzoy.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ldjlfebx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2eqfplusz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2dbmjhcah.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kqokmykc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2bhjxnlqj.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dgxbkrba.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2kttaxmbm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2tkxfefdv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zassqjjw.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2qqftpxvo.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2oazohtnq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2torbwgvq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ukovrpkk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dlmqlobi.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2teeilicc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2naxnrnsf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2lazkkvvq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ogiwlkyk.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2djxvakoo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ncnuljcz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2xlzqwaok.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2thpbwqdk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xfgqxmrd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2vrkohpja.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2jybwlaxt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2fvoudpxd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ucvsmofy.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2wpjkjqtr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wdjsqqpi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2byhedale.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qnlxyogy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2bgudfnhh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2hhmlnugi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gfzeevuf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2sklbjvwu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xnkyteuf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wwdyctns.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2impbaebn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nydakrar.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2hwqilyic.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ybeyimah.html


<!-- 参考信息 -->