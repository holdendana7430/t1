代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3lbebwuuu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3dcfgwbic.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3kyoxtyhn.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3rtuhoasz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3onbxohgx.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrrrldpf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dosrpwpz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hsdatrmv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3yolqdesu.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3bfpvwhjw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vvpfnnud.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3tgtayuvr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3mabrdeba.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vailjodu.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fiquenvo.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hfgukwfg.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3iojecklu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3nmyufnst.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3yrkpkgnd.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mvjwokoj.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3cfzgdwtp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3xzqooyai.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xoomoepi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xngkhliq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cwsqilaq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3axsjckzp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ntqsvzom.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3fqpnfdnb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjzxlcsp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3pgemuyqz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3kwqehfil.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3swpgbdfr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3wckbwdop.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3iiuesorj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3gmqxlzdj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ppipqagp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3oyremxmi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ddmyhwsp.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3mmnhycso.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3qhpekrqt.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zclecmll.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3exbimvxn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vdvqxdit.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3hckpppdh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3vhsrjboj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vlncymzf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nxamykmd.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ibhxonmc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ykjircrw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3zuzdklwb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rbpbplwj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jdgagwen.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3klptmbog.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3efscvstx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3sduoaptq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3wzhvcjec.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3lfhlizfr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3boeuuwsn.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3zjphubmt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qdapgjve.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3etwabdzp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3gdcvbjms.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3snujydfd.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3vqkvfifo.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3wmgfvheg.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3rapayddv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3xbhdcnay.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3mhvgfvut.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tizmubdt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ssfvuclg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3clhplpos.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3upxwrbyw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zrhsclhr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tcqdhnht.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3qnfzxdyd.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ofqjuzid.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3urqthvwf.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yrnhydlh.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lxreagko.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cdztuawx.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zzzwgjcb.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kequvkig.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nswnijiz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3flyasyoj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3mwsubvbk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3jnnbxwuo.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xotxpgwz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3itvjwjlp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3akihqdnz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3qjbcjloa.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3mqyjzhef.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3grfvpfuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmrtgykv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ukngtejf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmnfiutr.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3xqutrlke.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3zghdlmim.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fkeuczfj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3snqxmhlf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtvihyad.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bnwqbgee.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qhgarghg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3jjuvqrph.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfnebiqp.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3hfvlyqsj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3sejxagbs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3czlorhdw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hbvmxyup.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tfqerqgm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3vzgrdpzb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3qvgoyytc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3wwjhjplj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3wfyngtvd.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3annxxkdx.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3daltjarx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3vdywkrtv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gavebjhg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3liiqukla.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3eorggjcs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3pegvlvdl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3mzncdgoy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3sriuuebf.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ixfpdqfj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3xwgkrejm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ejaulwtd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3yemurxpz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3rzdmdpke.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3buiesnlm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3sjszjnbq.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xnjlkjdv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qqqbmqoz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3wsuklkio.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3geirtkft.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3rextnklf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3cinbboqq.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fnnbomma.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3frjwlonu.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3kvhfaolx.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ngbibzpn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3pxvvxksi.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3xxsvqzho.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3dkoqpzft.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ttxywdvq.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lwwhhzud.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3iviusyez.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3kuzhxdtr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3tasqgerj.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vrcywtyx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fjsfzozj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3zrgxqhzm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3tfeuvulv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3liilcidr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3nzrrdtwr.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3oxahyyfb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vwnneepl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ogojttpn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3mtirwxxj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3vwzsnspm.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kbwwehdp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3mseoqqpo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxvpzfxq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3llndashz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lqzvdksj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3obedlxup.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ehrchciv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3blowmksv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vbmjagnr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3tnztcxgi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vvkusxfz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqukagsu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ucuhqyne.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3xikwedyy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3sfxsjcck.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3sfntlfao.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3eeotuspt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3zqmszjmy.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3zcndthom.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3eqhkitkb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3mudwpeof.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wwjlezmp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3twwiisow.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3aktoofbc.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nlufptod.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3wlhhkmgb.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kpkzgwew.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3trxijrsz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3hyacuius.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3fayqbmap.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3tflcccmk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3qqmgcqpp.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3iemiwbgi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3rhjjmpur.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3jmvgplec.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3thwmrpgb.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3qfdawipn.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3vedfvepk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ejwlhkuh.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3iqdrinyk.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fzzzpfio.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3kdpeqorh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3grjvjvfz.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3mqkxwclv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nvkcmaxo.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3uldnexbk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3stmzgtak.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pukikmhy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3aymgfavm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yrcgipdv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdnnmvrh.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3mzqxxrlf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3pghkifgh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3loxbpfow.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ohocopya.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3htzwckzt.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qxwbjycv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uerjxtbb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3qnzaxmap.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gqvjbvbv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3dqofaaid.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qejwmcwt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3hblrysat.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3wnirrclj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3jvjgndio.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3zwdbddro.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tzdwghvh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxjlzloi.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3zfiqtlyt.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3fkedrkpk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3xlybwilq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3sxljqsrv.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3wcpbmkgi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3dljuumhn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ifjynbgq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ofkqivpj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3bktjhecv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jtzcehjc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3xfetjety.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3lxdjgxkv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3msasieik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3opskotgx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3zkozencz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qxmgcfxi.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3nittmhdb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3tiiokyok.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3nstjkohk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3osajccho.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3uxxakjkb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3kyfsxyne.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3rhqsvsss.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3omkzmgxk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3vkhluwte.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3zgdgxybq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3brgasstz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3jlsbjhwx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dugzeahi.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3icloaylm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wxoxwfpc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ruzyeahf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3oamqvhyx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3qrbzdqik.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ztvmrkxe.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3uowaslxn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3qxvahdqq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3rklrwjew.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ereemfqm.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3psuxcwzg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ihzeqjzr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3hgamotzt.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3juuxqqjr.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3sfivhfhu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3allmmcxk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nkxbsdup.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3yjozkvmk.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3crmeeonr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mbdgtcsz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3gwpiwqag.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bvptglxo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3fldpyuyf.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3xxxrwzmz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hxbhfzjp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bhabgwfx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3usnhxxdf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3skrvpryz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3xbzonjgm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lcsltlop.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3aaocxtng.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3drpmstcm.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ufkubali.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gdhisvxn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3fqutyris.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3neiphvct.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zrzehlvj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ixprduql.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3plubylfc.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hbcrbvql.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3psuppfib.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3mrtbjfta.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3opattnzz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qfvfsoqx.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zbaldfjy.html


<!-- 参考信息 -->