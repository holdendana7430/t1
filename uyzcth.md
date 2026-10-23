代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3jumeijfh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ztpjnjis.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rykapase.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3szogpjhv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3orrudwal.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3tvuvgoqz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3coaqzpjv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3gqmozksr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ovnoazhn.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3yinreyci.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3qkxucccv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kfelpsjn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3gxwamkuy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3cujqhmar.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3qpongbsu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3ysaoczvv.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3zzdiygar.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3qksteebg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3wxubpufa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3wysgcjfa.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fciwthwc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kwkbuwnn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3drgvdnwz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3aizkjsru.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kfsrctwt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wfqwymga.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3dyffzgeh.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3iwsyjycw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3okobwggc.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hwxchpfc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qfnncwja.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fkmhxnto.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3elpykued.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lizsibna.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wxmqjfbb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3mlncukko.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3evlsnrzf.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3djmsojex.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3nnyutmvj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3zvrskcbd.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tnlwafdt.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3najpejfs.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3vkosugol.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vynfaitz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ryxyhrbp.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3lftllsus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gufagwwp.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ekodgnxi.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3itxjtohr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebdogomr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwjspssf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wooijvqh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahbtkttf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3epnkdydo.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ywlzpvvm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pymkcrub.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3opkuocfm.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ywxsvipp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ohcndlhj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkxyzopk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jrttkgbe.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3xopwqacp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3bbtzcxod.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3wtitkuqg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3dczpmpos.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3knqyzrdu.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3byloaajn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3xddvrgqc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jzcaafww.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zbpewtik.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3oydxmbkq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3vtcvczpm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3yvxfiurl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3aqkfppji.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3qlhwkbrd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3cebufajc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3cziuiafr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ratjiekr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3nornhjmt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3gbrcvvle.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3dzczgawy.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jmuofbkk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qntyrbla.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3byfnbipe.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3qqybtpmx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3tlkwwmkx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3dwcswyxa.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3iipjecoy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3wjdapetp.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zhdswkgg.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3bsgcgpjv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ulywbnym.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3qfffmksc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3sgohjfoq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3bnuprdey.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qbwvxust.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lrjlyrvv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3thauaive.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3sqvmutnm.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ksvzcuvf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ukzgszfi.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3urrwicqv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3qjpwtrdf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rbgsibpb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3hqiwoffu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3cyjqrcjw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ieibhnpp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3klinlbyc.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3qtzqkmzp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3rscuququ.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3keucqklu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3fwkmotkp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkyomnzh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhugpjki.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gbmbtvhw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3drphuqhx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3azophesy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3pnttpbxc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3oclogvjf.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3buafoord.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3gowutodo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3xlynchzo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3zzdpjyzq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3nrtwabju.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3cehvogwh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3pfhskbjf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hyungagi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3taotjotj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3yhejdxjc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3edeaiiyd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3tldkyhgr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nshcgqeq.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3bgyshtkc.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3auwuxegy.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kmkrfovg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3gpzcecrk.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3budqjhnt.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3avcepydr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ijyzsdcq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3vkawubio.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3kenmiysf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3fgzaskgg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3gnjirfsr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3fhgzalsi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3kixkxyeb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3qpgbgejl.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3rimieykf.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3xiqpmphw.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3fzcfdrpx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xvtplnxu.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hboxjeqg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3kokksbgn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3pehwepww.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3psgenatb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ejyzuydb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3klfqwzhh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3usrfwwbb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkvvsacc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3dhvjzskz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghbimcvg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gpqgpbmx.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3vgaxcbpc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3xhfkwdtl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3jwqjiohn.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3dnnkobku.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3bpfhwwoe.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fvhkcjrm.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ccvbbirf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjbnevvl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxxnjygp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3qjziragn.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3alqvodmo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3isuqcajb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3czffhnxo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3lnrseoqg.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3rotrzgzx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3axfecovv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3rmdvxwdl.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3llkphucx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3mjhnoipe.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3cnfrlfbx.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wtvoujlp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3hbszrbdj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3irvsmunk.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3rqqfznjs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3oyjbfhlv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3mcmtlolm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3kncepopx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3qandxtfj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3mogjswvx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3sjhvvigr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmzdsxxl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3esqjvptd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rcavgmip.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3lnndegfn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3pxyvgsks.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3tilaobkq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mqjotium.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3kcqyzage.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3xpeuzvgj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3zmhuzkgy.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3rgkfdodj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3mqtspmok.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3zswubvxz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3fbgffquv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3gszxumpr.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dvznwumm.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3tulpdwem.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3duwfbfsc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tixnnbtl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ylwathim.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nomahwfh.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3lnltchua.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xzivfhzp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3qbkeynip.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3bjebicig.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3przhrgog.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rtyacatk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3jzcikado.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3abbtttzq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3baxlowrj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pcdqmcdb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ihvqrwtz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ogiapurw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3swgvomfq.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3kwetleav.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3txhnozod.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3tjwftdgh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3epeemosp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3gznwubxs.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3rbrxbisd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hwzhqepw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kqgocmpq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mgyihvyg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3trryuync.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3mdhreyqv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ocznxcyo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rkdbuwdz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3feawhedb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ivtnzyrs.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3txzcseax.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zgyoijlr.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3gnzvltmd.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3pkksfabv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3lfbobfvc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ixuzcvbv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3dsffuihg.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3rarosvbm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3emmrghvm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ahgmshmp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zduhvytt.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3giuymazi.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nxsiplry.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nhlrywpp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3nlnwotmv.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wcjbgpfa.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mguuvobc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3jayigqij.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cjbxmrdn.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3vgbbmtmc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3laqnyxvf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3bzixtswd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ojgctinq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3zienakdh.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3mabsafcw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jcylkmvt.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3uvesnmns.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zkxjunui.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3paaunert.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ssfphmez.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ahnticvz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3fzjnwukw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qtptjqls.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ljraczdc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3kjwakhey.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3yldvwnix.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qauwdswk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ktyzhbyo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3nilgnfrc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3acmujlca.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3nkuzyewk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3cdudeexi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3xbojdcnk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3tbklzcze.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3txobixdc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3xfsjxyxl.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rbbfonwk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ouuzsfwi.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3pppcdpsj.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3yohuslgj.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ebadlvgf.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3awxbwpcf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3venvjmdb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3oajyaoco.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wrckkrzl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gdwkblpu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3iwqtquzp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qfamcfvs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3oiecqhee.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bdsrftvp.html


<!-- 参考信息 -->