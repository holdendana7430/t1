代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2oucymgrg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2seaarjcb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gcciljrk.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2wnrenoin.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2unjbhzjs.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2hvienvkz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2muifcurj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zssbpngm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xcbzivqc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ekvnxnzv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2uzhoegsz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2xukksqut.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2lgkkuwug.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2beonuode.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ectmchho.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zbeoiwlh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2olsjroim.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2gxksfabo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2meetcafq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2pxyizjbv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2uhsfbizv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2yzeseaam.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2opuefula.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2pxrrifmn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yxgathmf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pxqtjxrq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2padstlps.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2rygsuvmu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2uausvedm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wbiktvcu.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2pvobgiwc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2cvrfgxzk.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2eoyfwqat.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aipxctqi.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dlayolna.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cfyyneok.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vijmqugh.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dknqcuho.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xbpsdwhl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2lvpsrfge.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2icbhygan.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2aftidpox.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ofhuiiwg.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mplfjrwx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2pcilqwge.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ibsmdbjx.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ljxarekq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rvlyfacl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2myztanzb.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2diflxpbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rzwryivq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2euahblev.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2xvjbuirk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2epuslrwi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jfleqvme.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uurrgfrs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2srsetcqy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2uryrrkel.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2xipbfbni.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ztqmdzpx.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gyzzjxmz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2bxjfrsta.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2qmakxheg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zflbebgb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lrfbuwxc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2mftikncr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2iqvhxzfp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2lhfayxbr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2nrzpynbm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2juzskuxy.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2gtfkvqli.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2imijypdn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2isnwjkfg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xjyurxsd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2npnxbdqu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2fgonbwuo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2skhsklme.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2uxydqtse.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2rbstfovs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2rdccjfpd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2rciyvlgd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wbmgiffk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2sstzedly.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2whdvulsh.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2dvpfbane.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rheulpih.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ylmmnwqi.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2nqzrvozr.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tdyopyen.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2xkcakfvz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2brwwzzag.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2xfuvfdjj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2kgbfixxf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2sbsigguh.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2uzgwoyhd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2mqnczloe.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wlhwwtkp.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2khghmuyz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2kgoudyxz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jvtzgflk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rubxxfll.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2jkcwsspu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2vjehkwua.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zlrlzeeo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lsqislpq.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2lzeznonz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2luobeezt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oidppqjd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2nquehruz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2uswzhizd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dyywlrdc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2esmdznmr.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2kmdtzxfk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2sfpcqgcs.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2qkjznesg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2hfvtspzp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2vhviubwr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ylwxjtmd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zkrdwgpp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2enshrtvn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2sjzqtkgz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2kdfciojc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wntsbfky.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2gvjwosud.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kvkdpvqr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qlhnrzxc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nexfkihp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2zfttgjpi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ejuyvtxu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2kthkyraw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2lhrtyaik.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2tjdoulzy.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wsyivyug.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2yudjqesf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2zeqptvuv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2pamrglnk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yyfqdbjd.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2yuiwclzn.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ivblazto.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2tmalfghg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lnhvnksl.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2trjdiccl.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2lstsqrnx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2jldibgza.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2mujoomtf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2mjitalwy.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2dqtmduyp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2mftycwwe.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2dqpjeibf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2itkuwdup.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2dnpvzxmm.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2cbeixafg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2wewztabo.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vyumdtyt.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2uwerdmbe.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2biakbcbi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2vlhmgyfl.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2cmalltga.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2igmsfeon.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2cvfurfas.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2mizneval.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2laucqwrl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2wfytlkxv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2erkznjre.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oeawtnig.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2azbrmhyx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2xubtzark.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2zkxeenln.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2xnadwghv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2dtxkcttc.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2efgtizjp.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2asllzbph.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ipyonimr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pvulghwd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2pykyjmop.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2asgxhiff.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2iqktsopz.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2fohpnaoy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2doxczknr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2mvyjnecs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2goydiimv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2shrvucvg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2uhiksuur.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2icdibujb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ymclyxku.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2lfhncbed.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2oxkpzzmc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2itrqdirr.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2rpnldtmo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2uiljfwwo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2gejjnxkd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2awgbjosd.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2wmdjtmak.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2npqycmij.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpteyerp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2csjhjkut.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2qgbuiykz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vmwdtycj.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2orclvstu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2lclundwq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2acbxothy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2iudfdpab.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2wpaxxbxh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2gjnulisc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2rjdvbuaw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2oqntjlsw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2mssnewkq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2finannjc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ltztbqmz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2zdrksumq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2jrqbfscf.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2legvhutp.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2zwnowsci.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2bwqxiqbh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2esfivydm.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2yafiatie.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2vvbtfajz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xmbvwdvm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2vosnaamo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2rdakbdfx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nurziepx.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cqsbhujx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2vxmhfrtx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ofuhdvzn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sddyukyo.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jfynnwzc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ocyayxke.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kysatlgk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2zhxdqvlu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dowggdwg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ukcswkfw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2rinlybvi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2masyabmx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2xxfkllhu.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2wcfttsti.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qmmvhjba.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zusybfmt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ytgxegzd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2uqitfkkl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ltvdmitq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vqxhtzfc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ocxwbiun.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wxbqfudt.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2brtyjhsq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2iutsbrrz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2yxwzccra.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2xeamjghw.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2cawbasrr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2fcmatpsl.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xtytjhfg.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2pmnzlpqn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2nviehiyj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2boclcion.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ybxqrztu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2zljtjxku.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ocdqsrne.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ocgfxwdo.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wnqduwmy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2vohhsubs.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2itotloqu.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ccvmkupt.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2zpwyalwx.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2trpzrefr.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2brnjfryb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2wqihkzdk.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2mlkdhhow.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lxoiitzw.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2plhuxxhz.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2yxlxfvoe.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yqahesyd.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2dsafbugz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2iuaorkpf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2nsrrscsh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2fdtykzcu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2fporoshd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2tcaaxflr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ezeruhlt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2uqntjsul.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2cckatwog.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2enqczamg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2gdjptcym.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jsydcuvn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2yvlwronb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ytitzkxb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ptomvrwu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2wtwvybkx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2vvadbion.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2vnmmfzsy.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2kijkdraf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2zlxrthwo.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mwufkyyn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2pqphzpyl.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2jammxjbb.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2jargikbl.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ishitcud.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2qyvetgat.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2tyixuhnm.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2burcurth.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2pekburix.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2tqvjvpou.html


<!-- 参考信息 -->