代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ykchabor.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2lzzyovls.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2eqfpyxwm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ycyzsqae.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2mrlcvixi.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ospumxpd.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2sbcoyooh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2pxjmwutz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yhwprlml.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ostfjeww.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2mirppled.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2wwyjnsff.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2cnoptajb.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ufhsndnr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jopawvte.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2erohhzqi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pnlbnlqs.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sntbjuzf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hywilbrd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qmvshrhw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tsmpkgfp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lgpammac.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ynrmweqq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2zjzfotef.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2sbwajpqh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vgtcoqaj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yapbtmow.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yuejbonm.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xoimhmlt.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bpunrlsw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ngcnyclr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bukssnuy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2qrwuenpi.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvpxoxbl.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uuqoroso.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2gflinrgz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ysktrhgw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2tkngbccy.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2jqkbhwnx.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xozyapgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lssllsbh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sviogygj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cuxngnwu.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2awahrsyf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2afbaupha.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2acrutjrj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2prdiegrm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmqodhbg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jrxmfifo.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2asghsuvd.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2urwbanjk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsfalskz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2hfyddpoe.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2fcqkmagq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pboertyt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtvjlamg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrlzbuqx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2vkajpdef.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2unzfeaio.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2watqimgg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2hufgjhvz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2gkyttjtv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ujvtulno.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2hufwgvjn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2iajizuom.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2linaznpj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2bextldrm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2vnkvvpsq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2vmdvnehl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2drgfdraf.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2qbufidpc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2jmsicgvl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2gqxbimzm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xbnlffzj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2gauuulsh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2djcggtgz.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2deqnlfnf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wyyimfht.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2faiorfja.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2wxyedqqg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ipgppeij.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2qrsjhmop.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2lqzqflil.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2efihfxsp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2jmfvpzab.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2wxoirjgx.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2agucwejc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2rrhimoby.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zdynpaiw.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2eszxnkpk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2sptfxdvv.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rqmyuuvv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ridsswns.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2allubxfv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2rwuscedg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2gozhodtj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xckhojpt.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2emebytac.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2nldniyje.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2mlogclnm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2vhjbycyf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2wophtmtk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ykgqdlzu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2wyqaeetv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2unrlxbkr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2celacwal.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2nnjgjxkl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2aqgzsdki.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2jbyefpnl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rlehreue.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fbqwxcrr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ozzvjnkw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2zkufyfwx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ljkyqbnk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2sesvcumo.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2oijxjshl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uclqiokt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ubmoqqxt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2xguuoosu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rpetldrv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xiifpiyu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2lnemieqw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jwtojcel.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2mxkdrjwr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2scexufsq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2hygubbrg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2zsvwbxix.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qagextqf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2mtvniuva.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2uklyaywv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vnpqihva.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2zsenchje.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mcxazshe.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2auncykpy.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2orbtuaxb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ogejxovr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2pcnxpycw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2eaydyhee.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2mryylqlf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2fdwlohtz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2wuwejkwg.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ssphjxjf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2jhxfhhdm.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2xnwktvtl.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2clwtisih.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vxohwnee.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ftwomomd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2sgkdouie.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2qvyisicf.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2bpfggetd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gmzwacly.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2descnhlc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kpedvfxs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ceiytbuc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2jhxyatil.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhuxqhcm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qmxkpllf.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2njkytrkk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2hwypjkhr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2covfacqy.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2utlimjku.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2cxjxamdo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2snmxeaif.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2egjbshvi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ecomwmeq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2nmakosyo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2qlphlxge.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2sdjyqrtg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2yqzhxvgz.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2tzhluufq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2hxwanjgw.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ilddltuh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2cnpqovwn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2iydupmve.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2csrzprqd.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2tesfrmck.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2orsuheff.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2tnoapwxj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2thztbrqu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2mrahxyxm.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2qigwllzn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ckoqdlsu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2yryvtjpj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2fwjkzizj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ryviodeg.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2nuaiwtqm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2chorajci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ztrtdsqe.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2twznttkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nsgkjcne.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2guwmvxwp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2hsjptwts.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2nmnbcuds.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2lhsynfmo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2imibpden.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2cfzcywdl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2kaoibwzv.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2yifxcktn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2afdxkzwb.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2yncgemth.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2xhkqvkty.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2gwgmikas.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aetnsvtd.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ubcxgybx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gepsdvcc.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2soskdmwk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2zawdnubt.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vhjasyox.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2rdjlainl.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yxelxlzt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2zpiuohlb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2yjedfqcy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cptvrhcj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xlifrlzx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mdgowqkw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2pfzmikjx.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wylowjbl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2oygmexys.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ndpkkjaw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zqlpowmq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2vfedpdot.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ealbbhys.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lcyiqjuh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2oomfbpdx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2wlwdpkiz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ogrjssnf.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2dvpbjbft.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zgqaqjwy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kbwyfzqk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2cnwpyuau.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2zphjzcha.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2dmsigmte.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fzvbuuyw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lrykfiss.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2baxyvxov.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xvsgmyen.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xokiiaes.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2golasvzi.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2kjzapvrd.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cvvilili.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2yzsjxijl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2reounyyt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2uscvhcih.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2fooubuqa.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ntdzceqj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2tuxzljya.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cuwpovsr.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fssfgnpj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pjuwatnw.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dlwcdjpm.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2sardzntf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qonfviqr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mqoosmhl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2epaujlns.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2gbwfhjlv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2zsbkzjjo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2beficbiw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2xonqmhra.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2xtbfgwct.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2vyqkmked.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jshvmutw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cltdqbma.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2vtrixkmu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kyxukdau.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lrmurtuk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ufntiqnf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2pfsiebrz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2oxtkclpg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2etubjwri.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zokgwklz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2agvtuily.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2mnqqaqcx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2voqcgmjs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ntdhyjkc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ntgdndzq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2sqjyuedy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2eckvtgsn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2snvhqojw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2hegbpwms.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2zyccghdj.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2kkthvgfc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ciaquexz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sxqhstsd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2xogoqluk.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2twropetb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2adourtbb.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2zflxtvii.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sinnvvmy.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2fmrrudhu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2mzmpiose.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2umlqwcqx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2itpyuaig.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zoapvyer.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ilvpxkgi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2tpamvfez.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lwqzqory.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ftbmvcyr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2uuizhvvk.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2xohlgbth.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2btdmvdbs.html


<!-- 参考信息 -->