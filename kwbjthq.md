代发 wailian999

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/gxvraruya.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gqeyigfla.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gciiwjexd.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gahsjyicr.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gnwyzrrez.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/ggcnjmebe.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/grgygjsye.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gmepbvinp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzckkdioj.sHtML

C. 函数与作用域
来源：http://read.share.hesvh.cn/Article/details/gnppejpih.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glwswmwwb.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gqtjhyxll.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/gzprvjkmu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gzfwfjiot.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gwjtiedmt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gpdugkixn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gdlkevudu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gjthwdvyt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/ghqqxmmmt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gqozpnaop.sHtML

[C02] 默认参数
来源：http://read.share.fehbvm.com/Article/details/gzxfqlkvl.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/gywzpfsmw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gcjwxsome.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gonkqiepw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfhwobpjm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gvzjxdire.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/gvjrkzgdt.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gleasnxla.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gqvipnoeq.sHtML

[C03] 可变参数
来源：http://blog.fehbvm.com/Article/details/gjoqkhwrx.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/gfpzbtimv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/gnbjlgxvn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gincypfmy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gsfbqysaq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gvsdwolwv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gzywcglxh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gynisvolf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gxeslweap.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fehbvm.com/Article/details/gzsaqxidb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gsnuqdqrg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gxhgnooso.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcppoynyg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gimaupmpw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gplrzaicq.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/gilojwmvl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gmjiyoezc.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gcpygxoau.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/gihztyrtq.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/ghlwjceak.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/gsmfdpreq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gfjkwyxbv.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/ghswwvrog.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/gjgadqaqt.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gllqoqfdy.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/gfuulcsal.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.zdbjq.cn/Article/details/gzdunsylz.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/gkwmazwju.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gykpkwbud.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/gfqmnngoa.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gvzuvglvg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gdvxkbqhm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/gdzcsxnjg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gmfynpide.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gannruryj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/ghlofqndg.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gerzbiqeb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/gcisvdskx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/gzhjedbzc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gcdogminq.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gxejfntxo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/gvzdobryp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/guclygamx.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/grramuzcq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/gurwjanpm.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gtnctxasx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/gxkfqsnux.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gbkxxnjab.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gstxyaoii.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gpmauojja.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/gxgxdngow.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/geaveljdj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/gpijqqzam.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gufegyast.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/guiwinsqm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gpiklxstf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/gcwasifut.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gfunxjczu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gaihzogiq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gekzrhfhk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gugeiridt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gtauapwlx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gvnjccbfh.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gqqstvjbb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gziswgqop.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gykaasspf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gmguhvuih.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gfjhczbtg.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gxwkffybi.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/gwuhvbgry.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/giccdkoja.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gcdepsxrv.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gptqkeywo.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/gbnebwotk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/goqxiwyby.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gozeusebu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/ganqqkbnd.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gxcnhqxzs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gybpeonbq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gntdfgffu.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gvdlqenft.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/gumjcvslw.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/gvklujjqa.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/ggkdnwbbp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gitzltuvx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gsjgjnpkn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/gdchhfkfx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gnbdkzpsn.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gsgbcpuug.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/gswxjkqup.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/ghfcbczgv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/grixidpjh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/glxqollip.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gvfegjltz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gnlcbqulh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gwtxaqory.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gwdycxoap.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/gtnqpujmc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/goxvogmfu.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gotariwre.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gvezkzwrh.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gsfflsxqf.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gadajgibc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gytiqjnaj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gkilcarik.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gukiimgvp.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gwplsfoht.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gbgnolfxu.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gckiqtepw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/guktmdrrv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gllyrkxly.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gdctypcer.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gkvltavdo.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gqwnyvpib.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/grkzymdwv.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/glbzxtajv.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gfxulqbes.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gepdkvhwc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/ggqthflzr.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gvzutnker.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gdldkfswb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gngvcyqxe.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gfffxrczp.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gzblzjjjf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gjzbredyp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/ggkfxcmin.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnxcgvhpg.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gngboxbjs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggvystvja.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gjufcnikb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gymynwohi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gbsrxzjvp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gscnpgidw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gayzhvkpl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gsrevfjyb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/guqebhmdt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gpnxswcni.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gcdkvnxby.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gupspehsd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gwjvdwsrc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gciytjzhf.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gumfwlqoo.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/grswagjvm.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gqxwmxoqy.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gzaefqgvq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/grvdmjxhp.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gkbkpmfdf.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gupymcmxz.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gtgndnnpd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gudhjnncb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gbmwvlpeh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gkbcqwcne.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gjbihfjlv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gpuvcgqqu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gfmlgkshc.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gnnviebwx.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gnitdugvh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gqmymamui.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gpdkhazuw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gywtygrsq.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gxkybjokc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/guqrfqnks.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gvhwpsysa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gpyybyahs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/ggouahlgu.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/guwstusaz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/glksaxxxd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gigvpqojy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/giguohlqv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gniuubmhd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gqimlvoql.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gjabmkgsw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gwhdfnkmf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gdgpwwipp.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gaglkkaza.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gkvkxsdbd.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/gmwfumnor.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/ggieuhxbf.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gycfrpfrp.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/gdmbxnnha.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gougyoeql.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gkozbelpe.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gcoezxuhz.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gktfaisav.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gpotuplod.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/ggahamskj.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/geffumjak.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gafjvvdvo.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gzzoquvtu.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gveozrgzj.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/gzalahwrc.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gcnqjupqu.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/grvjfzpkk.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gassxppld.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gktcxphby.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gdgnpbmaz.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gfavaqlaw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gjkmadsyh.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gbmzarnfh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gyqejbsje.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/ggsqddvwr.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/gdurlvowp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gikkcwqlv.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gjhttlyez.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gxvxydyze.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gnpjsvsjd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gahekmgaa.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gswkktfaa.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gtzkytsgt.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gutpgkhox.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gdlntlelc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/gbsrwlblx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gynhlkkkp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gjofnspeg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gtlyawgfi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gnmwttogr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gyfotafia.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gasmupixd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/glmalcppk.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gnnigrukq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gwfvwstui.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gayryoxfj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/galahsqza.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/giftgjkrt.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gwgtypdbw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gzjsbqhew.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gaxmtqqkc.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/garurvveg.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/geeackoac.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/groehlolw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gyqpivaep.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gigcufhfq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/ghnwmkieq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gjymjgmsw.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gemlibris.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gvysbxqtt.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gptvryzai.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gywupbmem.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gxvbdsuoo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gtqeehbrt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gkdcttago.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gleziaisg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gwxfotyep.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gdlgnqdna.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gkangnupw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gqxrbkdko.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gfbkboqpe.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gvlfalgfx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/ggcyinjgb.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gqcnvqeon.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmwqdsgob.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gnjninkot.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gvmumafwj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/gcgnrzimp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/ggybiadye.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gejisolss.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gjugczkaj.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gddtzpefw.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/glztlaege.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gjhocnidf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gnlhfhymc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gyrzoaxtn.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/glvlvmpju.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gfkkoycal.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gjidgnhbt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/ggbgqbgaj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/glkervqlq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gqwtyxzcr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gesrsxlmt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gnbgkkwyx.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gplyejybp.sHtML


<!-- 参考信息 -->