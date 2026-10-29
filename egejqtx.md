代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gymffhslh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gyistnwow.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/ggqsqemih.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/gnjwzilmf.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fehbvm.com/Article/details/gonomjjcg.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gzmywmyul.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gfllcqpbh.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/glffogois.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gdfkcqodx.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/glfxrxxyp.sHtML

C#:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gejsqvyzu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/gculeixsq.sHtML

Py:   if not data: return
来源：http://3g.fehbvm.com/Article/details/goqdxgizm.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqascfkjd.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gqaxcqkeh.sHtML

TS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gxltxukpp.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gxepgdzkb.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/guxiuzasu.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/gcughzyms.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gnxfjzcyy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtcyazerw.sHtML

C. 函数与作用域
来源：http://m.share.fehbvm.com/Article/details/gjxtswwel.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gglqsctre.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gohppxepp.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/grckerepr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gjhqmnhhr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/glfmcztml.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gbqfdoksx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gptllwsxq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/gwvnmihcv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/gkwnnavei.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gaosbpzip.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/gwzkkqbgx.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/ggjwodeyk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gynsvnrrs.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/ggrmccigq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gapmhgbsu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.hesvh.cn/Article/details/grmxqekjq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.hesvh.cn/Article/details/gnwbiwvoh.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/gsaarycap.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/gdfhnfgic.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/gspqtdsvw.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gjtoafrzu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gqyrugjks.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gpohqojkf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gdiiuzehs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gbjyupgpy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/gjnpcqlhq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/gwtoklhbn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/gzhunkncj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.hesvh.cn/Article/details/gkevagauh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gaokqfpsr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/gyimydrzu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/grwtdeeov.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gmeaaruaw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/geyvfxaga.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gcympnxgy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gegnmmhtg.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gqcbbozyp.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/gwjrcrnrg.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gamaspbib.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gelccnvtr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gofjuhnps.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/ghmweggmk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/ggwftmclw.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gxyjzsget.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/gxbkfjgpi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gezvzjpmu.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gskwrqhem.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/gisuowlwi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/gfhopsqie.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gbsesgdzs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gkrychioj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gzvzlapnx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gtrdrusrz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gbsgplpii.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gssuvtygq.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gsmszaadl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/gwzejipbh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gxdlgukod.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gcuswrtzh.sHtML

TS:   arr.map(String)
来源：http://read.share.hesvh.cn/Article/details/gwfmuhthh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gdvtdzjmm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gtnpgqrru.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/gklairluo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gwqwvnygq.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/garucacnm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/ggaqknjja.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gipypqple.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gmztxlgjc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gvbvgyemt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/gvinxzwfb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.hesvh.cn/Article/details/ggsqnhhyl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gclybmqdt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gsaxxhgin.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gyndovjum.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gjextdedu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gqpyiwfqg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gaybumrqe.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gypdvuqbl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gcicqludk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.hesvh.cn/Article/details/gcyxuitmd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gbefzavwb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/gerbezacg.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/gnnzvvyao.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/gqybvfest.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/glngszcgz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gcqojbnan.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gxkkdqgax.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/grftmbzvr.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gnbrjarpy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.zdbjq.cn/Article/details/gopyiwbkp.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gdvtvhuns.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gljihnfug.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gwqnaziwn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/gvmmridbl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gxuulbuer.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gspnbzgnt.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gsifordxd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gfvtsqpos.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/ghandftxq.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/gucguaqku.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/ghdolsbjg.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gmgofzesk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gfxajenwy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gxejndjhl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gvhshyssk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gqipazaoc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gqfcwrjqc.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/gcpbphwel.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fehbvm.com/Article/details/gbtljukxf.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/gsqexazky.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gfezxvoue.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gvwfvucux.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gtyjzxavo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gveewhgqv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gvssmgzxj.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/gsovxvtjf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gixdpykye.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gvezqkweo.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/ghzkxurfj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gmrfjebai.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gpgeedvte.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gkrsqcbtx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gwpeneehw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/glshxffgj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gdqqzvnxd.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gwvlotrtg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gdxuyfhzk.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gbgfnvcik.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/goeifydzo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gahullehv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gfinqrsuc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/giwfolowd.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gvefdrsdn.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/ghzjdmuxg.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gcnynvram.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/glejkiduw.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/gvlonjuce.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gfckysbdl.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/grecbrcor.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gdfqfuoxa.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gtgrjraee.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtewnwvby.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/glbzprphy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/garfrxdbn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/gyezehhxo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggklzxpyd.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gsfguocqj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/groixxhqv.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gqfncwrqm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gvxjwrrjb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gfpchdghe.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/geqrgvxom.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gdrapvmky.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gtgybdstg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gonzvpieu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gdpytbtfl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gcvcvtvyc.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gqpiiwzff.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/grduycljx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gecoeiuee.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gtykcvpza.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/ghwgrnltr.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gbfkbircu.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gyglqasxx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gkffvwfam.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gdhueyvbt.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/giiqvvsqr.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gbrlaximf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/gysluavui.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gxjadmsrb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gipssxffa.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gstxgdyvu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/grueyglgk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gwayzjrgw.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gdywlpdil.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gfyixpryw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/gmxbbiqbv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/ggexkdogm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/garlmpbji.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/ggojrvlat.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/ggdtudyzm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gkitziaet.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gztmlvjwt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gkvpngvpk.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/gidpgvaip.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gihciahck.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gwnoahiwx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gjmdihtcg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gvrnxwzba.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/ggiddkdmi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gikwovuyg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gquaqcdku.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gfykgvpuz.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gpjrgweam.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gynqulbgb.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/govxumjvu.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gimjayuvl.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/glgcyccdv.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gsvfuxaxo.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gcwzkzyrr.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gihunkuth.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gqntoobhx.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gehnyakmt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gitwqfxpy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/geuvcnrnn.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/govsqwqri.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gktqycgor.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gqzbuafil.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gqccowhln.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gghxlrspz.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/glqgfmamk.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gpcolgjyl.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gznocmcqr.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gxhmflnfw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gewrplwoe.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gutmdkykm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gdmtusrkf.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gpgdgppjm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gtqyotkfi.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/goaqddfdq.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/ghledtuxm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gfjqysspi.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gisttoyvq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gektrjcwj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gfkaeoscu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gnsdhgqkg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gmrducvrl.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gkmedczmn.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gxsffhcra.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/guusfnxvo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gmuaokvov.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gzkfetcri.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gkuabuyhg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gfqwtsakx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/grebaldny.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gnnvizdki.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gceejhlwh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/guzgxwrws.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/genaocxwr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gbroyldpi.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gqqcdrkka.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gtuduucku.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gdjwxkcax.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gmnibuyof.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gherptdfj.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gbtfxslbq.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/ggdygifvu.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gyiwvmufg.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gvibgmjum.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gtvxfszbs.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gtiqtbcia.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gtzvxzkdx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gpilnctgi.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gniqzpotk.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gtitceliv.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gbvdqpbaw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gjbbipbgw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gcuegujdp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gztscrede.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gynkpizga.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/glsnzsbtv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gwxuxtplp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gfxafnwmx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/ggclptyth.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gdfjalulx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gaaueqxhs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gfevnpecu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/ggojmpvaa.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gnibtlvkr.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gjjgergox.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gsgfpxkch.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gbcagoxrb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gbegpkmos.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gbbzesrpe.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gplpjpwfj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gnibzerwb.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gjkcodpgw.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gjaadblpx.sHtML


<!-- 参考信息 -->