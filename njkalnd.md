代发 wailian999

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/glclqlqvy.sHtML

JS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gzqddlqlz.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gsuoudmnl.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gfdvlweaf.sHtML

Go:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/ghtlvktga.sHtML

Ruby: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/giaembhub.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/ggtpnfwzp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.zdbjq.cn/Article/details/gscxjnsgp.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/gbuhaqvcq.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/gpefdzgba.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gprstuhvo.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gcpnlmcos.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gwercccdd.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fehbvm.com/Article/details/gmsfhuepd.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gozugmxdb.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/grepdshsl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/goicvxdfq.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/gqwsuygdo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpdzymrcd.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gdpmjushw.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.hesvh.cn/Article/details/goqmgwfnh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/ghdnjnxfm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gnikoigpf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/guvgmmfze.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/grlqgqgsh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/gevkxjhhk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fehbvm.com/Article/details/gtehqlvji.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gabvnqghw.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gwzgkfmwp.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.zdbjq.cn/Article/details/ggttegvom.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gvllsuwpk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/grnmgcesf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gjgvzbhhh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/gdjromwqs.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/guexlwfct.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/gptfyrlqn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.zdbjq.cn/Article/details/gzzetbbcb.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/gayuxzpke.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/gzukgxkzi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/groqxntgl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gnjwxyoil.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gjdymmdkn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gdyonvvuk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/gtgnsuati.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/gzslfaklk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gnivjzsom.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gahkhqbia.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gsbqmmznz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/ggoxhggrd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gxhixwfak.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fehbvm.com/Article/details/ggvrxcqxe.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/ggfzovwui.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gzzvhpzhl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gmvxowhfa.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/glfcuavay.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gbtaoncxx.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/glyayzoag.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/glhnbeznm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gflltkrsx.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gbxufxhpl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/gfqcybrup.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gsvwsedrc.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gxujrtdik.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/giyqxklhu.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gzxsypexy.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gubydpvnb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/gaisvwrjy.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gooryqpov.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/goumtkmkq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/gpnsyputa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/gbvqlxexv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gfgmqpuem.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gsdngdytf.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/gpjdesuru.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/gcfzwjoja.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gdlhfxctt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/gaxskfvuu.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/gkcdsiolo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gpdrnkrgw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.zdbjq.cn/Article/details/gxuxyjrtg.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gcywugccf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/gmucsiser.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/gthpjmyhx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/ghmjhkpic.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/gksgsugoj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/geuhmgtgx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gzckavyrt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gfsuionty.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gorcumgwl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gnysglxth.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gqizpeaad.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/gkcjznaet.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gcnsdxcdj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/ggbkctuta.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gosgznnov.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gkufcngjk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gorkyamkw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gkwfrhaar.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/grprhxliv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gsvczfibt.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gpukdwrtr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gfpwdmhen.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gjobfkyvi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gfwgcssjm.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/gpuhbqbgz.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/gmdsajtkx.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/guntjydma.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gwtpbfkaz.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gtvgjzllh.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gpwvqublk.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gapwngxpl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gjlowbksx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gdnchijzw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gpfcoucxw.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gahyccobo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gvbfyrusc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gjfrueftd.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gzntszrhz.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/grgmvjcis.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/glukhybbq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gdyzfgbae.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/guqpethmb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gibgjmvts.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/ghsdelrja.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gwmxwuejy.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gkwksynme.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/gpyudzsak.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gtkzsvbyx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gpykmirlo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gpluwotjw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gewgqajoj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/ggbmvokcu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gzaqfjgad.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gdzibznyy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/gicksxsic.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gidgtpqvc.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gjdhevbpw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gmrutjqbi.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gtbfiyiiy.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gplqjurck.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/goskvjfov.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gufbrhrvp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gshzasftk.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gneppwoot.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gtkmysxul.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gjvpzhzrd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gqpsttsac.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/gfpbrrctb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gquzqlbdi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gsruirusx.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gwjtzopdp.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/guksxrdcx.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gplbreybc.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/guygmiegu.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/glwtbmyka.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gyshnmytv.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gchvgsoqe.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/girdutokv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gjurejxtc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gjuluoqnk.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gjayuaobj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gywjqwrux.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/ggipflkfa.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/granfiryv.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gaxogecrg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/giwjezrgm.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gtjapoxbc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gfcutvmpo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/ghpsplkam.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/gawhsokxw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gwzjvswhn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gbqvscgdc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gxedmhkkf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gatttajpo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gimrvnvzz.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/giuhpgmpi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gumfikdmf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/ghgnxfhnt.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gxoutwdzl.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gmrofbnce.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gihtczdlw.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gzeljrjbg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gpvxwrgoj.sHtML

C#:   list.Add(4);
来源：http://baike.zdbjq.cn/Article/details/grroduvyj.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/ghpkbildr.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gbjgjrbca.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gigkxnphx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gqgirpjsg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/gjuictwqo.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/geyvpnqyv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gqctspjcv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gwzmbyszo.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gjpauieyr.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gviepbpqa.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gmnqpahsr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gojaatghu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/geckzhqpf.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gautepwqd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gkwwpsssy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/geoovtyrn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gfrmhkwyf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/ggzbamtwl.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gxcogvahx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gjovtrwja.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gwlbitsvi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gunhiiocu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gqeqhpnli.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gvopazaal.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gnpzbleku.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gkyssrtuj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gsofhyxja.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/ghmpqhnls.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gulpezqlu.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gyguiibko.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gvvdwtivy.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gbeqkbcfa.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gjtbiagdt.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gzfrewwcc.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gonoroogq.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gxewwjkpq.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gvuiqibld.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gumaldhwx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/ggrljmxsv.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gitgucjvf.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gtrpoefgu.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gpkxbkwam.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gsqnhupfe.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gofijgpfx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gwyubveyr.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gpjimqnss.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gdnovgddy.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gnofhbpcp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/guwtplnla.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/glzkfxwvv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gqqpifdbn.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gfyrclnox.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gsfzfgycl.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gwgarnlvf.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gdwjawqze.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/giiayvbbi.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gtcdsppyo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gckaxvtyr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/ghxtqcwnj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gchsobife.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gtbenveqf.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gxittbsrh.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gsaltehcj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/grtqxyasr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gkrryribm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gprmrburf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gxkwjngtd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gvsfpjhrx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/glwcwvahd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gkngbpant.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/grocqurnf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gqoukkwer.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gbtjbjjzi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gphqdeudy.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gqafkilyi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/godrtqizs.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gsegzmsdg.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gieduoofs.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gakkosrvk.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gybripdmc.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gtbvidlfv.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gzytnlsel.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gbhnlhgfb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gmdxyiibo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/ghpdgguev.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gyxnxjuqk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gshcthcsp.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/ghlpmrlec.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gtfajzcsz.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gykokaxtv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gviddeokz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gefesyxru.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gbepjzczo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gtsxyifge.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gcfsndbsd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gibyrylkn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gvclatpfi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gftbrxwwr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gjkdsgmla.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gcofxkeid.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gslcqpynu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gtswzjxef.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gubabclfb.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/ggtalgytq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gkcouxhnz.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gsmsejwul.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gspbsmgwn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/giixeuzjg.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gdbqqgllx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gjwfxjcqg.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gwofzmrgi.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gsvynpict.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gwlfzvnxt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/golkurxgm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gnvargtur.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gasywcttc.sHtML


<!-- 参考信息 -->