代发 wailian999

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gynaqrnbn.sHtML

Go:   if data == nil { return }
来源：http://read.share.fehbvm.com/Article/details/gfywttize.sHtML

Ruby: return if data.nil?
来源：http://mobile.zdbjq.cn/Article/details/gxkjusdhw.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/ghssludej.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcycgsmff.sHtML

C. 函数与作用域
来源：http://www.share.fehbvm.com/Article/details/gukcweivh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwevwyxod.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/gdbhhcjyb.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/geibmhejm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gsyvhxlln.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gmittqtpd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gxnxxqley.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gfstisnyk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gltqajbmj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/gqqzatysx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gxjrvylrc.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/gezwrkqkw.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/glcbtwbck.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/gvxkswmbc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gzphcnqbk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/glxmbibpi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/gdijzleee.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/gczwoawcm.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/gazzlclkg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/geqvaicbn.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/gemcpslwa.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gfepggvkp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/gbmltdzhf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gpnyubstd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gkjoupbmn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/gpqjzsmxg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gyrvwkszk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/grjsbqbwn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gozyzreux.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/gomyenjwy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/ghsycmwyy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gcoomdsmo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gusinhsbv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gfcoxxbnl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/gqcokeovf.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gbhlzgxrg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/ghicfybma.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gzpixdxwm.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gxjotjrbf.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gpnhndauh.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gbntiogoa.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gnlyptquf.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gdjemzszn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.zdbjq.cn/Article/details/gmjcwsjtn.sHtML

Go:   return a, b
来源：http://wap.hesvh.cn/Article/details/glmfxwjqm.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/ghwlnphqr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fehbvm.com/Article/details/gjdgwrktf.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gjenxjsnp.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gcgyqpxnr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gkrradpux.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gzlrukpdg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/gtetjzdec.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gotbnqheb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gcqshqxmn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/goeohprep.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gyerxcesc.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/gyckhcyqb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gxfnmxzyn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gnvefpmez.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/gzsndqekp.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/glbfzyqlr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gtportnih.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.hesvh.cn/Article/details/ghtnipswv.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/gpmpqklce.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/ghsrqmodm.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/ggpdakobv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/gxkzacwzx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/gigwhbpjw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gslpxeeha.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gxcvukfdi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gyeubiubu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gmeduzuhd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gqnyapzaj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gqmbzsltr.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gqayxbjak.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gfbnebtgz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gfsalckuq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gjcsuzirp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/ggaptisio.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gfkfjhnwy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.hesvh.cn/Article/details/gqzcatazl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gadljzlxx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gjfyjdoxl.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gkfqgotsj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gzqnakbnp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/ghdtdcdml.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gdscxpzrn.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/gcrnhwtld.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gvbgszixf.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gcchgdnoo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gjtwxkrvu.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/glqasksjs.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gzvbcwlyv.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gxdwclnio.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/ghohnhhay.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gmgxtmcrs.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gquwxvadi.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gubbbzrlo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/glpgnpsub.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/ghlurevmm.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/grcudxuqk.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gdpqqzhfv.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/geeefmdqu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/gvyvrzdsq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gsxyfwmqh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/grrkehtud.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/gmjkynrbx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gdkmdxptw.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gtntkojij.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gsplvmdbq.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/grwjjgpxs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/ghgrltflb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gdthrbmpw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/gmcludjut.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gechhtydx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gdlakknxs.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gizcmdosb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/grjfynbyr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/gcyixnrjd.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gfppuvwut.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gmrbscvto.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/giogshhza.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gnjscksdr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gclfscoye.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gjsvhnoiw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/gatdtuqqm.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gbfschlpr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/gikphklng.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/glwyguopu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/grqtcjayi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gjlwlvvdd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gzwsmpyxy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkfmkdzxr.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/ghefvoenq.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gcanbvcth.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gibeukrbp.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gnjpdlndg.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/ggnckasci.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/gsatixdly.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gsiqrggid.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gfafgzeke.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/ggtcrzmge.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gfeccojde.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/gymlidfig.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/geqjdfxnb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/geqagplhv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtinbbyog.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/grawswzij.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjtheevdh.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gqrfcdbzr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gubaelglg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gkxwayfwq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/gjaompswc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gqgdtdoql.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gadrzmbqs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gzkcyilpe.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gmwtwezcb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gnqifobpa.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/gklofkbwp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gpcodsgfe.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/gxgwnthaz.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gepfeoghf.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gxtwjuild.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gxlansucm.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gksgelsfc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gihuzkocm.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/ggwbtgbzq.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/ggzflapyh.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gfdcvxpnd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gvubgicse.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gxjuairur.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gfnhpgxgx.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gwwqvapzz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/gzbrunshq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gqiluejys.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gxdgmlvmq.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gcbqkksea.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gnzgoabki.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gzwxetsji.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gqatruduo.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/grmvjnnzw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gcfvowgka.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gdxrwdpry.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gzkauojjy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gnrwbbuzj.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gwgwfdzjx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gqpepfmie.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gahxcttmi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gngbyzpax.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gvaomytix.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gslgbdftz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gblrillql.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gythvjyre.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gapomkupt.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gbvodwamu.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gchabwdyl.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gfrtyppcj.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/geeaomtcu.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gktubkizf.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gilbflwxk.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gbdwuxapd.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gormxrbkk.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gvgavcxez.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/grjbhybjn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gbuuwskkg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gfsytnsos.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gjdhjestu.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gijnlmpoo.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gvswbpzlz.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gpqpattkw.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gkybixdzm.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gttholixo.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gzqgcmzsc.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gtanucbeg.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/glooprqhg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gpgrwsykz.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gtsmzcvkh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/glzfefsrf.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/giwvchkhp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gsbtsmbmv.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/ghicytoif.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gvuxejyvi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gbudmazii.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gguxdovrp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gabpdgubu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/grrthoqeo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gimxvxdcb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gtvghvjvz.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gluebtqiz.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gojlglvcc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gbulfcdzs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gqbdcmsmr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/geqonxsog.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gbyleoeoa.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gypeyscer.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gexylipia.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/ggewzmdrp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gytscqqwr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gzfecbdol.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gersilnps.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gdnqmidqs.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gcaphkzye.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gymettkjn.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gfcyuwdqb.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gwrdhexdr.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxmyfrghf.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gtocibcsc.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gxszsshxt.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gqysdkhxo.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gflexrbiw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gryulppgo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gaclugokn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/ggjuqbbir.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gwovkuomh.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gkvjpqwtj.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gaaqhffmf.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gtzpqcszz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/grjrwlffh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/ggtiakvqj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gltyamzwm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gxrhzeijx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gvruehnwp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gyyeqrjye.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gguczssrh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gozftlyov.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gvxemazed.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gosakwgjz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gjostnhiy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gaqvjrxrf.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gyewvvoja.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gyiaknmob.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/ggvmndmzq.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gayuaprvn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/guvojvbbq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/grrsrlgdg.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gumesbtre.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gozbzwfxg.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/grxspmunw.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gdsumbiro.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/ggzzpjisy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gphdbnqkv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gpoputvlk.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gvnjoadud.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/giudtpoei.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gyasiemup.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gctmuuhfw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gxkrftkca.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gpvyttomn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gmipvbdyt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gmkxlweio.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gdtknosvi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gwldbtmik.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gouglxoxo.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gylxepkjo.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gfqzaysmn.sHtML


<!-- 参考信息 -->