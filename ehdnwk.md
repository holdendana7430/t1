代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rcvzadzt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3yhjefxwu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3lmhgclqt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3utxtcrso.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3aohqjwvm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3kdbgskco.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3imjbytvq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3jtmfeuwp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3jraikepq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lnrlnzfm.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3oszcfxzl.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ygbzecce.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bmocbnyq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xxrhanhb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pdfvdiqx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3cynltlon.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3muzeunoy.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3gxojtwfi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hfztaeky.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3tpjstimg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3poxuehdl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3uapckcwo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ginczivq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jtngjtxe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wzadwkgd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3fuqyttlj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ndpdinxf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3srutqmzx.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ywjyrisv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3offcctmo.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3kzzxdidh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3nnnadyim.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3goyjosth.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3sbsohxwy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3xfccrfoc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3fizpfqvx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3hrsivvbm.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3bvvwjaeo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3kxippcsn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3istudfpq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mcjhpvtg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fbyzggpn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3buvovaji.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3wffgewvi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3deeyrsow.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bwvpbcft.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3obdskbwy.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3cxsrsctj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ohxmnnnp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pwpfzmle.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jbvmqejl.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ciynzxpx.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xuuzwjgs.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3umkkdoim.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mqxiyoum.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3duatzhhl.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3hurxblwo.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzltmusr.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jafwlcbc.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3upagixky.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qbfnjjaf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3yxzrvcme.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3qietyoay.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pzfcxmwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3irywxolc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vurljfue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3imxmzxxz.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3zydzskbb.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ifyjmbht.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipvxoozw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhufwelj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3arxvnapw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hvkpaoox.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3onutckef.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3usrrpzyp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sctyoawi.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xhlrylfc.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3kxstwwdk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3kziamgij.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnkmtvxq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xeotdoht.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3funsqotm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3msixzqpw.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3xpyrehfw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3eljdbjou.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3azueubii.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3hufepjdk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3gylwhmyd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3akxfhmtu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zwlylsel.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bsaeeomx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3pzcfsvlx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3drwdqbgy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3noobpxzw.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3yvjwhunw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3lykkjtnk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ifcdmlyd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zqjjxltf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3yoloxtvi.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ioaochxn.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3hluegnpe.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mgdvxfgk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3epzhjucd.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3caqtsvft.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bjisgpcu.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3jnkgrxcq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3kgjqfypb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fgxudxpe.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3hcpcvuai.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3nciorlxh.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3xhzirkqn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3nedptnaz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3tqqcobiz.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3tzcpzxko.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3xndrjrif.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ckhwtmtc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3iaauydll.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3pjrbluuj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vbcaksqr.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3iqykbknq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dbqbeybs.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3xohjuzbo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ldpbdjbj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3klafdvkd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3bhkzvvto.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3myxljlcg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ilftobwq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3xofgaeld.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3puxafhay.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3xdeztvtu.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3mbqealqc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3iraluspy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbedegwk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kerxttns.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fifydqox.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3lqtnujbr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3lppgqoca.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3phgekwxr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkghpsoa.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3cubywpkt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lcdwipjj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3royreyrk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3byuqmxbm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3oksdplqp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kxsihzxt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3fxxxgpce.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3kmxulaxi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3meeijwcy.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dbjhyqbu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3owfsxgsx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3rdmqimub.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zgpwqwte.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3txvbqhzv.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mxkxeedt.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ooxyjiuk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3zzgtmbog.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vtzwnyxm.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3rcfuazqv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3twouphuz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3nfsaywkx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qynznykq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3arwmdsqn.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3vgqxrlwb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3zlbuorec.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3soyeaihg.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3dapiyjmh.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ckziujyl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ucxopuqc.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3mxabskxq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fswjawwz.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3cjnscvhf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3poocipco.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3jufbzmbo.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3zvksqcqk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ycnoewqg.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3mvexqvzp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pwgmytko.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vcurgeel.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3suwnnyta.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qwguouku.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3agqizzti.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3nccwxmpn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3jrkwkkkx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3qpmhives.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3vkfnjbvk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3cgrqaynm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3yxekdepr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3runlvyib.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3fpzosswg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3mfdgeefa.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3vprpwtbw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xcjqbijz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3fkdonfbk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3uqtugrqo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3hpukjjdi.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3twkhpopb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3atbezuxl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbfvlsfl.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wysiigjw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wilcguvo.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3trudluio.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mvuikkjl.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3icuqarno.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3lvzbnysn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3hagoknwz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3bcastirx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3hkekxdrh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pkfgsbht.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3kfoaufhm.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3qcmioaty.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vuhmllkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3soenkgws.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3jewuhirk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbwkzbrb.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jvizflhc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3aaqyblok.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jjjzabxs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3dxouotza.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3yrldngev.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3aviujaik.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3oabrlwdw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ybcchjmx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3yuprgczc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3miocbfid.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3uddxsvtn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3lopysqez.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3dflprugd.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3fnschttj.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lexbljcr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3kloxaekk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3cjxxwfmx.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3awklaypx.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3iipgxoug.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3yefifgad.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3olxcpjjb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ehmaxelc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ssabaayi.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3yozzfecs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3xjqjajww.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3rgqwxnfk.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vgwqafbb.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3miyimhxl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3xniyvyqj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3bbxtplmo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3hbjruscl.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3assupeqa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vwtvoqyj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3tswxqxij.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3eddunese.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3lbqjrisb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ldfboszn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qxlttoyx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ylnorzqs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jzassngy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3rjaqucjo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3qejqiidg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qmyjgecj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hhzjtbsj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qfqejwru.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3lqivqakt.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nteoqmlr.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pldymbmd.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3csfsohrg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3porotxfc.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3nqzejbqb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nqkfbnkf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3epnnuwnx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3yyyzkktj.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3nphuuvng.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ssxlknhy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3kopexhxe.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xnutvqbn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3eubheurs.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dmxjuegp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3qpczpfew.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ezmipqkk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3arvwnkqq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3dtuveish.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3bsgnjujg.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3pfunqexd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3khjoyeph.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3qvyhuatb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cnwlvtmc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3awsuvjxr.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3vdvywknc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zpwoockp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3leauzizd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dogqepko.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ldoxjckf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3qwubiuyx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3kzlmqgoq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ipsucwbf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ivhdqywt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3aeynjjta.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3brcuqyml.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3jpcfydsi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bsywcmzs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rauqpbje.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3dzgswmei.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ypbgqtlg.html


<!-- 参考信息 -->