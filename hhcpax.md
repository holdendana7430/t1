代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2zqdyvjqt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2kfcjcsxw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2xterpgqg.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ahffoqqo.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2qmzsgbgw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2etomrjxd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2btjbedfp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rngdadws.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2jfjapgby.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2zwzytuag.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qtpaycuh.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2zaciygfz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2qesuataf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2tzdvamxt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jgaamear.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wdoibsyu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2spluefud.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2nkllaiqp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2jklcymnk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2djeewryh.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2pmcgsobw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2eyoxotik.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2sjsrcgcu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2bzpflziz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pxvccfie.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2miwnymxf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2xaeyobxs.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2yfksywca.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2wevknceh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2bjicemrn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ryrdravs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2mnsjxjmh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qlzwaoag.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hupqcpfr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nsudqhuc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2fkmcdmol.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nodhyoyz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tqybwyxy.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2goxfnpfl.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2jyadumke.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ixkppfxm.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qyfybtcx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gtdpybek.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lntmdmtt.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2itoicbiu.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wzscwdjy.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vuswjbqh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2hwkqokes.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2giwykyca.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2esurvoaz.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jrcemijc.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ggbqtfjr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ysuephqo.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2braisbww.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2sgfazjcs.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2jqmaqqax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlwwqjbf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pgfxfdzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zhlahkej.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ipguigyf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2upsavxgk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kalxlumz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dzdtljdq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2klgulqww.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2huhytsmn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2shzfczmg.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ygvkhnfv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2csfwaewp.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ynkjudfo.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2uhmylstm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wecigwjp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ckbgyxng.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecvqvpyf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2vasqnhnh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2kadokxkk.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2jsfhqkpk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2xyczxzos.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2nsckvphl.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2sxbowxvo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwixgvyk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2jazcpxpa.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2akxpcpxz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2muvtyjtr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2nlfzahow.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2zsqfudkp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2phkvcxmk.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2kobvjffz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2mighmhgg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2dcljnqur.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2majhdzkq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2lnklsejx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2sicecjtg.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2sdvqcfrm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2okafaljn.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rqqbwtqz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2xbcfupbf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2sphgkxpp.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2euyzclkn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pchfkocy.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2usfgnpoj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2aeymlqed.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2pmurtbkb.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ubmtpxbg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2jxujlzmr.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2sppdhrle.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2tlcpikwt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2diwqdkhw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vanhkhwd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2sdefmmed.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2opjikorr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2hwdfyarq.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2bymxejax.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lfsnnbku.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2okrtrpad.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2nnenxbjm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2cjvtonek.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2dmotxdoz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2rslnywif.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nobgkcrv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2vdxkvels.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2ubdkccln.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2rluhnlxn.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2uapvueix.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2fypfplph.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytjqyqfg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tazgelpo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2givlbqcz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2vfoeyjbf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2dghnfymi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2yzcihyot.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgkejpxi.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ehavjzey.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2uxoyztlc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjtstkmx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2fjfcdwnx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2gdzlvpvg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2kbleovau.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2hgwcrvrc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2epyjmruu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2sxtmbbxk.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2somcqolh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2xaczvdiw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2zukhtxbl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2vbdvefkt.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2owkehonb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2imnezszp.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2btuncdjd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ksgkagwq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kkrnodwk.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2zjjjawmb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2znsgxapj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2vkggupan.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ystonavg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2tmykraaq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ngxvrjyc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2hcpxefny.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2btuhcjao.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2twdatpkw.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2mmiybzqn.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2rfrbjqrt.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2mdxdwezj.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fmvxkugt.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2embhxohy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2hrudnmqg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2nocakowd.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2nrmyityp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2gkbojoyx.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2svaslceh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2egcblgwo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjpgmldc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2cjurltye.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mkdofdmq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfsvxaie.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2qxesrhbn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2tqdvpmsu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2eamthykn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2wceqzxcz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2zmghqron.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qdppfbyz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lyrxchzl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbleoufq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rjfubfzv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2vtevxxpb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2axycwkcx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2wsqagyvq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2spkkejir.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2vsyoydvr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2drbkbgqr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqumebsd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxycohay.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ruzwtdui.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2bqhefqxq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2zpciqzda.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2errnasqd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ndetqtdt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ffprjnrh.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2vddfpokm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2kkohsidb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2prvzixvo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwaeiulu.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2dohojnhu.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2jmaeaszx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2irflfchi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dlttwmqj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2vigoqcde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2witwkomq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tzwqvlaz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2hsjbgsbo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2dmsamwgp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xzclojbh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2xhykifyb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2fteuogxk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2gmtuvltq.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2agsllqkh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2gytmufek.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2suvnloam.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2yvvyjkxd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2seakbstr.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wppbvpmg.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lgzwngyd.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uxuzilgg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2klbqvlni.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2yfbqdyie.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2hifmfwnf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xuixmyzb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lqzmfzbd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2dxswuvnl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2fjdxmwib.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ybwximfh.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yltontwh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2gipeervg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2xsuiujpq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2luhhowbm.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2mjqchlsm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2twrbtiez.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2laeoivqp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2wjnewrlm.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qkmloodm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2xekrwcve.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2avvreiha.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2cnqtxkti.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2kogosfqr.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2qvlqgcli.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2igfwefoz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hyqposon.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kplkqbjf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2vujmdakw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ammtoyvp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fksmmxvn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dohjuqvr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ymelurhb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fgekakrx.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2eibjmbhg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lugtcyhf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2brlghndc.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2biootbej.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2axtdtcus.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wiqjykbn.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qulmxdqr.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2xhaoeiif.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2mbznyjgk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2wtttlfsp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lvztjgen.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nbyqdjtl.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dthudbwz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2egvwbleq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ssldpriu.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2mdhlpcjb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jiiywiyb.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2umhvktag.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cevlevwl.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2egvmzxqr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2yhmyzuud.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2luhswhvx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2annbpboy.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2fyechqud.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hsdkgsaj.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bqbhlzmj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2uabldnfa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lagywngr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2buqegdho.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2emkdynmu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2jwpfnkfb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2gocbrddc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2eqmkwcra.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zlenuhel.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2sbmqjrps.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2johupjlw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jpssciqo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lvtgdjcv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2pqhgiovd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2vwbvrksy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2inlhpwuh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2avgsexrz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2pbypcxtq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2quniuvoe.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ppistqnp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2iefffyji.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oifgcpld.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2rbymgawn.html


<!-- 参考信息 -->