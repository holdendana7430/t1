代发 wailian999

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2nmfmdwaa.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2mtgvvjfi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgfhfxoj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdsroydv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujrafise.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnuibvbg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2lsrtdfek.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2vhekqtnb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jhlvolhv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2rpfhikcb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2nbaiaeyc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ikzwinue.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2wlnvazzd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2yzyiuomj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycbkwroy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2whzlebdh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wacgyxyy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ecuvmodp.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2hmelzrop.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2hbgrkgak.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2jshqvpih.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ththklza.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nkzcnypr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ridhgojy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2kynmtapz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2womnytns.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2noijqquh.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2fpahsjwr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2pvqepzlq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2zxsdoypl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hkhqmxym.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2otopcviv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2suzxxlih.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2jwiqjdwc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2gertggpy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2pcdqvzqi.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ozuwtuvo.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2wirfkfci.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2igonmpop.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jrjxtlbm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hppjepjv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2waxtjpur.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2suemhupx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2bsdduaye.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2qedrnxsc.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ncircjdb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2iorrwoxl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2xppagmss.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bewyzswq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ttveqkmh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ykemhzjn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2zzouexdn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oamwrbdj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rcxyoqsa.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2noiavrju.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ibaqmblh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2uvyhzsid.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mwpdacaa.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fcuynjdp.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tsrtysxj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rmtyplvj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lledyaed.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rzzpiqec.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2lfcjkuym.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2upuxccnk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2gsznjous.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ooyxbqrg.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rhxefbqf.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2aqjttwkn.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2cqtoewtc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2lycacifm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2plyjnttl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lslmhwin.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2hkbyxhtj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dlmtwnlo.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2xwiigsyq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2heummkgf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hjugkgql.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbfgdhyv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jndwlpid.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fvjvtksr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2trmtcbve.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2eseqdvrf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qkaumutj.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tyopkjbr.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2zhjvomhx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2doqtacmi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnxdzoyp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uejifuki.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2fogflqky.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2szegyxvu.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2zcatsyjn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2dvoyvbev.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2bjjdmzpp.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2qmhymlkk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2bzpmovkb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wgxvwspq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2cgchyhpg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2uxzmbnbd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2pydhugve.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2eqovegjo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2rscpiirw.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2jdtgnjtc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2xovyingi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ebajeyxl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2eqgqjoat.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2fngvapdt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2sjrqtkvj.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2pftmvdrl.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ozfverfs.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gwhmtfwp.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2xckushez.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wqgdcocw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2eockkuxr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2tzycagem.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2mluatblh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2uodcdkos.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2njbukcdi.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2qzicydic.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2gqxvawyd.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2dnpxqufi.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2fgrxojeh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ldgdddjh.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2drlkezaz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kwaukett.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2zeutvytf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wkjindux.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2gdiqrbyw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vekkhkkc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2myjznqxh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2looikxue.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cewvwwsg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2eacskemv.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2iritvtah.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2woplrisr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2xekghjie.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2kwxaiqlc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2oddrqfux.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2klnlxvxy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2axjdzkzw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2howezobz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vqbhdqba.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2akvvzzmw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2omprcpzx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2kpgftzic.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2fyyhsqfq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gfimhjfr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2jmdwsssc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2stfyrtll.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2fdhjbxuv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2txozkcwa.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2fifhfucq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2aedfkgfv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2xuxzmujn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2zqojueei.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2nohottxr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2owhxejak.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2cisljlpx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2xxnflaap.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2fywflmpg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2wpuqxlpy.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nfjvjiik.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ybnhmwld.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2wvbsewri.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kfoyzikz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2tnxbpupo.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2xccpdudv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2mnekvzdq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2eggpiteu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2exprsszj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2bglxwbju.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ztiavitk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ldkkvjyg.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2swespcfc.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2wkryrtef.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2nkevpmoo.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2wecayuks.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ttldcrhs.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pcdthwym.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ykpoenor.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2muhnebvm.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2rxiojptp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2hgvtwgst.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2jdbfwjbe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pngxyywm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrguqfsj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2pxcafuul.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbhptayg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2meorxxev.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2avhreflx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2qgggyicq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2mxxhwigx.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2wkoxdhig.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2jnzfhtja.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mofrzzoh.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2picvqwjl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqxvkkyj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2sgdimrxa.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ecbblvjd.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rswdsklz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2bxbdtsrw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2gmmsdqbg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ijpgpytg.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ngtxhvqq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vqlenuor.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nulxkozq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2skhiaypy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zmnwihax.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2eqkxrqbj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2rgjuwfpd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ujxpffks.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gpbqsmaa.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2llccomoj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2rehwsvpu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2iakqvrcz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbbuczxm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2fqtenaxj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2lkrrcfrn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2vsuyyqns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2itapjjxq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2lqmlbrmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xdyuclok.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vetaxlio.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2zusxwzji.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2bohacjjb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2kmggqemi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2tijrqior.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2fbbmmkso.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2fzdtiaos.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2xdyvwblz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2vucvfyat.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2orauoubt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2xlkufbqv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2emlodqzj.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tzgkoiml.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wwijhbmf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dqsnqzsp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2uulzryzl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2wmmihipa.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2tqzcmfbx.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2wostnlhj.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2qnqplnvu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2azykyjou.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2jlggzzxy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bxhwpkvn.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2swzeoijm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zbakjaqo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2bqeymmkh.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zkppmfxj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2dszfnavc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dpewdhjs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ngynfhvq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2gdfdynot.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bamvdjpf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nsexsizq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2vmxhdytc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ydrmrudz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2bilysotw.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2rxvqylce.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bxdlowrv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qtczksyq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2sysrnpzs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2zlwrrmvd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2cdhodlpw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2exqeghid.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ixsrdnng.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hxxblrdp.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2batiavpo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2acwineiz.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nnbtzobm.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rnfppezu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2uqadospz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2xpunsiof.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jddfnjub.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2inacfgcj.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ohzyuojp.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2nizrbrgb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2rcofjzfe.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fpopvjej.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tewiqqpv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jwyjvuut.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zqxidfjh.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2kgagsxci.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qkaasosc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jxrzqpmc.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2kuxextwo.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2gpzkvixe.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2lrigdwxa.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2hsjhgrwz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2pzeiqwfw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lgbbcsrq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2sqxrfotr.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2euvggpsz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xfdpqwre.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2vlheidij.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hsodzcbs.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zugqqrqd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2drecfdir.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2phwzlpkd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2fljiebzi.html


<!-- 参考信息 -->