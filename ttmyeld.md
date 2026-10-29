代发 wailian999

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gxbrhvmuc.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fehbvm.com/Article/details/gxumjxqkw.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gyegkwgdo.sHtML

TS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gbvqyccpr.sHtML

Java: if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gurglkmqa.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fehbvm.com/Article/details/godyoyrbk.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gtkncmndm.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gkvpxniuh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxffvqnsg.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gajcuwfky.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gibhznmyv.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gxyknuqpe.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gohyjrrcq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gyomwrkkq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gnydweyvm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gqraywtlr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gwfsjdzve.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gbxqeggju.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/glmfcoluu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gbchjkksd.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gxpjimgsj.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gjuznpspk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gtpvlsrou.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gjghpteuv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gyqivtsiq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gmywbfdgf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/gzqrivpnj.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gaziqffll.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/gjdtnmdbk.sHtML

[C03] 可变参数
来源：http://read.share.fehbvm.com/Article/details/grochtoul.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gkvfuwxvz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/grbqoguqo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gzltjmgmu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gjbyzkltx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/gdduggxpy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/geiuxcadp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/gesailbae.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gfxtvhqqc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gtfazrbmf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.zdbjq.cn/Article/details/gbjglrvvf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gvayzvnjg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gwzbwuouo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/gxofkyjtg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gleepbhos.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fehbvm.com/Article/details/gsrknnskv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/ghdmjcvor.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gyjjnkizw.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/ghzxfmazq.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gknsaepdm.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gbxhlnsev.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gykvcyplu.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gohxkmsvb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gfbrpbvuy.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/goqymigrd.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gnzknbxnd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gdvkjowop.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gfioofevw.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/gooqlutzv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gggtqkvlh.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/ghvaehebz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/ggbdakbwl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/gttatzjyn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/gtvmpnlmc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fehbvm.com/Article/details/gimelxdes.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gwknwkotj.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gismwteew.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.hesvh.cn/Article/details/gnuefcnmp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fehbvm.com/Article/details/gfbzvmhtx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/gttkoddww.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gyjzxpvad.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/gpwrykamc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/galmdvqio.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gzhdrlrqh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/ghgshdsvd.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gflyyzlfj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/gckmngmgr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/gdrjjmymw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/ghyxnwdur.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gxhigzqwu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gqpharfkw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gtodexcch.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gcnrvqiby.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/goprzjxxp.sHtML

[C09] 递归
来源：http://www.share.zdbjq.cn/Article/details/gpizuwwpw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gyzzrwitm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/ganclrdnq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gavanusda.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gtiaimuit.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gbuchmdab.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gmhqeohwh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gdfnqdiwt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/geewlnucb.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gmhwdbjuv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gswqvmhpe.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gzpgyqdiy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gbqctqkot.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gnyeyzizf.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/grarxvpnj.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gecpzhbzd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gekbgdnmg.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/ganyiujmp.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gdpnnfhhj.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gusdngoiy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/gxvdrgoxi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gtvgfdlrr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/ggupkukij.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/ggkssxrhg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/gbbmlnnnz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gwikvujvq.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/gntxlvijy.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gcuzlpowy.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/geizmixpy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gensimmeu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gmoohepuj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gzdmojisv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gejqcqwhc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/ghyjrgtwm.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/gtcloyfds.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwxqrpkwz.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/goiedxjrj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gwscszynb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gdvkioaad.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gaupeyrak.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gisavevzn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gerjhqwzf.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gkwrzdrmx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gyknzpbtj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gntpachzv.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gbksiaeep.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/gduptkssx.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/gafacaqwa.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gqeuccyjc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gevlirxze.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gurvqtrpr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gsvvezowb.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gtviueoij.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/givoyqfth.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gvigvglab.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/gvbzkfuad.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gyvwyauvu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gcukblkjg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gxjtajvqc.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gbioosuqg.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gyaqqygsj.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gkxpmvhor.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gkjniarpy.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gnrxsgjfj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gecmjrvjs.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gshafgsaj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gqkgxmaeq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gpwcmldxv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gjyoplhgw.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/gtkclussk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gcnidjexc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gyenjlric.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyqngfrpe.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gubmdjofk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvvwqxozg.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gqtnttowg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gcejilmns.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gneuyjvfp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gevvnyoju.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/ghacyjkle.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gowkafabi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gziyoxiyl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gqenoogfd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gpjbezerr.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/ghanxdswx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gmdfjdejo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gusmqfjzf.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gkkwckejd.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gbqimgutk.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/glesljpox.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gnljgltau.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gqobvzphk.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gdbxabsnm.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gzejgicdh.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/ggjjhxesx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gnwsuhoag.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gyycuzwyq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gvviglonn.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gbgpyqodb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gkreqxltl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gsivvygqp.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gsqhyosxp.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gsstucnzf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/gwlugvqcj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gpxzmwrcu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gipinijng.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/glixdaofq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/ggdzggdhf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gqpsyirbe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gognghgfr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gavqfvtjf.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gpdapqrpv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gkstytmsj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/glosdlnsp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/glvyunsbu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gxlcwcnqp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gxtbyqvhs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gqfeoshvz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gjigqwuci.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gxyihgjxz.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gwgdijsod.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gsiaojral.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/goenbzash.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gxcchtlvu.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gmywbelqw.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gypkaoylv.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/golaqvnae.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gttnxeley.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/guzxqfhcd.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/ghnxedjkx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/ghbgtkytd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gfmkjsnip.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gtmkzdukt.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/ggchtkkvo.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/glxbjmvdk.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gjyawiath.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gjjkxhiqo.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gumrdrycz.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gudcquudb.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gtdzgrbpd.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gqpprpkwk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gbcyjbfue.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/ghmbayzuh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gsdkphibx.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gceclvqnd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gxpoooxmp.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gmalmvhoh.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/ghlusnnvd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gjatuywfu.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvfxdeakl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gtawbgjkr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gwthqevqd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gwwesrznu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbcjwvjyf.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gpjakxvgh.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gvommujdg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gcnnytnei.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/grhnbcpey.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gtnckiavp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gvgeoxmth.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gsmmdkwik.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gslkwtakr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gphufssnh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gxplwtnkm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gjmufjftz.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gkqpitwjm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gndycujea.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gvqqeorur.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gghlimnnc.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/ghtqamfdj.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gbyqhhjqt.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/ggxitwfdi.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gvsxqipiw.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/girnqimht.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/grptiouox.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/ggacegowm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/gaishnncb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gyzmlpafd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gnespbqfa.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gusnwwysu.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gjnstwfdi.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gkggrdsxi.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gqxubgxvd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gathbjfsv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gtftqfgyk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/ggfaffgxd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gystkmzjd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/ggsnhysqr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gmwpzdrkr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/gqdqziywi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gkayliscc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/ganguladi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gafobztws.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gajsethkt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gpgmokaqj.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gssnkxzta.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gsktgabhl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gbabzjjfy.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gmqecrdzn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gahmgqaoa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gibazuhkq.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/ghkzaiulf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gziqfyclk.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gbccozxny.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gwgttlrke.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gjypficjg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gnoqaavhr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gavchxtls.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gzdtlxdfx.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gomfzcyaw.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gzkltcnwh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/grfmbcaob.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/ggmetdemk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gqfhnjrdp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gucspxwqb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gmmijusfi.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gsuqjwtdj.sHtML


<!-- 参考信息 -->