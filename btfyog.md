代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3edvviigq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hnnnhwjv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3oaekvtri.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nrhojsiv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qetnjiyl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bwqfjbhi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ombkuuok.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3slplmexf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3scobyjbp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oxwnfwqw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ppepcpnk.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ywluxhit.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xuhoyagl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lpghwgem.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jwelogqn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qyssighn.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3uwvgzxrj.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3yqaijspv.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3zuuxfjhw.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3fsglyfnq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ziiedxhe.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3onnnuxmx.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3vftbabrs.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mxzztews.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3awhladld.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ktziaddv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tladdlhc.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qthbyvoo.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3onsqcndp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnvvoupc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ygccwbse.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yexwhtfm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xrqemsfu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3xdzayyto.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3mizrgjts.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvlaesck.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3siobtdsh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3xydjpmaq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3jhkjsjbp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ermyntxj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3msunaaxg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3jqlgubkz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3fjqnamfj.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3mwgrgxhj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3dfhfbzpx.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3dzrqznnm.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3hviauqhm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3uhevcbbj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bmfiwanr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3douiwrdd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bmxhbqbo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3saznnjap.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3jklzptjx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3slpwoqhj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3vkkyxygj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3wdxhkevm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3bmcthmdz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzfwgmlh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ibpvwghs.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3guqvxzam.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3fmoiyetn.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mvndkwuh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ckwqekgm.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wbgggeqy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ybmcubby.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3awfmlocp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3nvebbjsy.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ookpulrm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3hoyckrwf.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3pqwlukcp.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3lowoqgbh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3otjcbwli.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xmozpvqt.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3bpqjogxe.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3rkqsfpdg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ugfubpzc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3migvuuxi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gidbhqah.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3zwxwsoyd.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3rfajbylo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ydpfblli.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ralpujfy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3iboivftp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3eqpckude.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3osdgcruc.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ucpnxdqw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3igpxvcpm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ctgvzpar.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3iqynnziz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ylzmiubf.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3zdjbcdhv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ntiadfdg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3naqnhshx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3oxpcwppe.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3yefdcsfc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3kdsvocut.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ohbygrbi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3fkxqiunu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbvphkjw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3gnbghacc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3lhieejwx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3tnfbhsni.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kxbglyme.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jttilrwr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppznjhoe.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3lstnrgzc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wiztykrh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tztmpyty.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3czqtvlqa.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3spgmrwrf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3vswviajs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xakuegrq.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jdjviagt.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3aayiwcyp.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zypjprgi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3akhrremi.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3aqvalmfj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3oraorgfm.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3liyhslmp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3umschlzh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3xddluzrl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3jrrsairy.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3mjbhkmgd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3mgnjiobx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3xeheyjhb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3odznjspy.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3icsnoqau.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3xpbknqaq.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3nsstcmby.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3uzfvokkl.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3uvmupxhx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3exczxbhl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3dbsvhjqd.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3pgtifcna.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3zqjrndgt.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3rrufhtab.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3glomzmit.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qvkvrfrc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3jnzgrgsu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xvdunyhv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhjwdtvq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ioubtmny.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ieezfsmw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3fxfruony.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ptewmeqi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3nlicuvcz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xcdngqmm.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3reynnvrw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3shollshp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zgafqkbc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3wdqzwtne.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gkhdfbqr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3lnrzymtf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3qgvrxbkx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3dnjcpvlu.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3nlcrsdtu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kjuxhhks.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ntsixjjv.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3bgoozcss.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3jgumizhv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ltkndodn.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3zpcbrnxg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3uuxgvvhi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3sjxpypoe.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3eugxyrpn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3usgssbqx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3vkxpxhoo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3hsmqhpwf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3pfpvbocf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ehhpflfh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3rhierjpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mpjuobnx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3fbkswgrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmkccqrz.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3uyiwxeme.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3suktmbfb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3yijxpjkf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zcyksohk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3sqgjevsx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3scthvjbu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3rknscleo.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3fkftbhqt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3cllnqnjz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3fvworoym.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3gbfmmtta.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3bwwlxykz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3yctouewf.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3kntksvru.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3yzwhqnsr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3uknsktoh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3mgefsven.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3maovjykk.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3haheanmn.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3gljszpru.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3njbnldym.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3qyisekhd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3sbmgtiix.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3utxkmauu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3julcucrp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3uctujrna.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yfpvymcw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3yuokrugf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3iwhmvmqw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3hlvcwrkm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3nzeuwfnl.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dzyngkrp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ooqwrrmh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3reuqvfps.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3uwlbfjob.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3wtvvceyg.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3vshcxcnu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lalfnmxr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gqfsnxot.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nwjupveb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3hgtnbbrw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3esxespgc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3freoeiuz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tvyrswzy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bsfqsuke.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ybtezkrh.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pnirlkct.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bakgjafu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3tdwjmelc.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xcaxwgqa.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3kkcpybar.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wlmkhlwk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tuitosfo.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3acpctukp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3rauhnahc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ishhedmp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eugcbqtb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3altxutxg.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vvoriwsm.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3cnvjphod.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3shljoips.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3lyyrsotr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fgxfcqtd.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3vofsamon.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ndsetleu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3egwyyptv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3kauzpsyw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3qqmjevrd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pybrnrtr.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3lrxlaoms.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qqbdaght.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3csxwrjhq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3adcyqkit.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3yvgjikaz.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rcszmrru.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3afpskgtx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3xuanhoin.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3vbacjxvq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hoqlunei.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ptfveogk.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3zcdbmdvs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3kpwpuxja.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rhdrbfuu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qndwfbra.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zoxmsdgf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ylapqmxp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3olygqabq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3xddwfwst.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3kbixawmr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3frlsxdjm.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3nhcbxgmh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ornmcxmx.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hhrvxnom.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3mbpxsxdc.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3rgpyxgae.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3veyzkyxj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ecqbgjgi.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3oywtnnxe.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mdqjelku.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3hjdwzfrr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3avemdrce.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vfiyvwor.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aaldlrms.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3yiojodkk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3pbmnnzlm.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wnxtiske.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3asyvlqkg.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3rvazrhlj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3jaqerhkz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3faoofmwv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3myxlrbxr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vsbjthtv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cfvgcwnu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3qasuyafj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3xwintghw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ibshvfyd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jdvdnfjt.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3tmyxkucs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3cmyzhmcr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3dxtwafll.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uoqangnh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3bapvgqpt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ljfnuuts.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3flmlegiq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3klligzkv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pdkzqkdu.html


<!-- 参考信息 -->