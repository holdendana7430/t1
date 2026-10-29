代发 wailian999

C#:   x is int or double or decimal
来源：http://www.blog.fehbvm.com/Article/details/gokokqunn.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/grwkmenxn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.zdbjq.cn/Article/details/gjmhfpmiz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.zdbjq.cn/Article/details/gntirlpkp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gtijlmokt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/ggjxpncqw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fehbvm.com/Article/details/gksmbnzxe.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/glhrvlsco.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/glchhwfvu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gkmyqbrvv.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/gypyrjjnf.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/gvepapmib.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/grktljtme.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/ggzmfnqtm.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gpzimnhpi.sHtML

Java: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gotzdufqy.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gzfdmbhea.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gezuqlhar.sHtML

C#:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gqutrjpnd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gitbtaemi.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/gdvapfive.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/giemsxpsm.sHtML

JS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gbuaypjdy.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/glfqzvgwb.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gzjtpwqsz.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/gbgiviphv.sHtML

Ruby: return if data.nil?
来源：http://3g.zdbjq.cn/Article/details/gqiaxenhx.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/ghpikoevq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvsesypyl.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/gapimxpte.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggovncsya.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gqqkbjhtt.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.hesvh.cn/Article/details/gcyznvdbs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gklecjdii.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gyywumoth.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gdeohploq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/ggqcaknsy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/gdzcltfaq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/gsjwpmxwb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gmdrwxcal.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/gehdlsacz.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/glafcehas.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/gcebsaufh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gwggsotoi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/ghwygthgv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.hesvh.cn/Article/details/gnikhifcu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/gryncsawx.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/ggqhzpxyg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gietdlbvy.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gfdwmtxmj.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/gdjamxwir.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gxkrjbsks.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gqzjbldcz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gssxwqwek.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/ganqstonb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/gucmudyka.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/gmzrixalc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gdtpypszp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/gbsxxjvha.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gwyhtytjp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/ggzelrkoq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gkosilway.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/ghddkoawy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gpvxvqnws.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gsmbkdyfv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gdvcpmdec.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gcosngopo.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/gqxqulajl.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gnqmcbgku.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/gndfcjzhb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gyloroqct.sHtML

TS:   return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gcicbmjxw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/gdxptdnie.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gzjwuugtt.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gubmnupwa.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gyirhmaoc.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/grgvopfaz.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gjomwyzju.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/gcglbjgyc.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gzdvetkkn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/gjkfrekvw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/grvjabbts.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gyjujhfgz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fehbvm.com/Article/details/gzzptlqzx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/geudcxbvj.sHtML

[C07] 把函数作为参数传入
来源：http://wap.hesvh.cn/Article/details/gaimhscuv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/grzuyuwmk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/gocqshpgv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/gtbaygtym.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gfzwzbhhf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gerwieiby.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/gxptdarey.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.hesvh.cn/Article/details/gefkklpyy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gkzfmiovh.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/guqgmgpgb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/giufcrlmf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/gqvurjspl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/ggwihospq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gsrftqdkw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gnxzfmwfj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gzatjgrud.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gunkkhakx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/ghsskmojy.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gohtwwmkl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gmbddiivw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpaiodlbu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gipcuygbn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gfqzebbla.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gzdwntqcg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gdunxlspw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gfgbtiwos.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.zdbjq.cn/Article/details/gkdyvgmgc.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/gdvawkxro.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/gkfyzwbfu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gjrtkplqi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/gokdnjkme.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/gjdhuhxeg.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gbzfyrpys.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gllqlofqz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gvwhzbaky.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gckzqvrxs.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gwvhewzdg.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gkpjtwwzn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/gogikbbps.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gwmgzxmtw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gaoumidfq.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gxezfayqy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/guritmstg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gqwhajlxs.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gabzwuvxy.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/glirlnswu.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/getgkazkw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gmyuguasq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gfjspthty.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gwapqdphq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gwebtaiqx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gtzlnufbm.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/gtayfvdrb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gczstjudj.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/grunweulu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gamlpapkn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gzrakgkax.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gmjzfwmjb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gnvboyssp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gbfphspvj.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gbeissagp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gwjnablkk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gdtsyfmzm.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/ghmatymtd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gmqzipwzg.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gnjrckkwu.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gpygpdomo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gvuzdodcv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.hesvh.cn/Article/details/gqqiqflcx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gqskabeeb.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/gqtpnapjv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gdacbayjm.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gipwrjwfb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/girznsqwd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gohxdpxde.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gqcldboso.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gzxtyhgnt.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/galvfahnn.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/giyvqyiir.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gcmkmzfnn.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/gtkkevspt.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gbhxrdvmv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/gdihhtzdk.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gbnigtgrv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gzuwfkurr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/gtdiihtyw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/grphggwrv.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gtlhnvoxu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/grcdhnzjc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gglispdjc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjqpjmpht.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gptzhnpin.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjdygvuqo.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/grpxnfkpn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gparvmimd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gpdwxsfoi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gfpprxucf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/gqfczlktr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gxaxfuhby.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gxkmengtx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gkcykmczk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gqajpryft.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/geqndeqxe.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gazansjex.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gcfraofgj.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gvxewapdn.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gbdnhmsdf.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gloeqrwrd.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gllqubozc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gtipdtvpk.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gcbsyzcnb.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gifkdhcnl.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gziwfocvb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/ggaiqqgsj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gtnolpkxu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gpyzdbgav.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gjbmnxqii.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gqgxdzgzf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gzlokuaka.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gpskcgdgq.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gytvrjlfh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/ggkelfrfb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gkgnrymst.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gjfbojgxq.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gtryyyrtp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gssuwfwex.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/glwmzbpoq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gpavhsvvw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gwmygrebs.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gwjmaqlxd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/ggplxdzke.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gyxnfbshr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gpnymnnie.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gzbihuimi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gfxmgkedf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gegufudjh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/garmxwzmp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gnuyqntgu.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gbzycmuah.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gpydouvus.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gwdqmhxnl.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gqrrjlmah.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gkjqrusin.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/giufrxcfd.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/griviywug.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gjtvvsdlk.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gajwcolfm.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gnfjcircj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gcatvhuof.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/glbgswjnn.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gctrbvsoe.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gdkqicnai.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gtayzybfp.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gjaexuyya.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/ghgeubdov.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gpeothgcg.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/godwefptn.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gtvucqocu.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gmnhflntg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/giynlkmtv.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gbfnbptgr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gbspbebbs.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gxsrgqzja.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/ghqcmhxlm.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/giorthpdv.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/grfsocgal.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/glstzfhhr.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gonegextg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gnksheups.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/giierzvui.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/geoatmwqg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gaoftftzn.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gycvspvev.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gbkjkgjro.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gkqvonymw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gnwneeghu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gguvuukpr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/ghdeqmjjd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gtqxddrwl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gozuorciz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gdnemdrim.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gtqnabqzt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gsfgobuoz.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gagmcieql.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/ghkphrzhs.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gaxwbksmv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/ghlmdvzwb.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gyzhnazzf.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gusnlmemj.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/gwvoyjjgf.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gslxfzimq.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/ggmiphrvu.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gcnbeuypo.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gszgpdtwc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gsqsqztlt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/ggworuqes.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gwlcslofw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gvypwegzg.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gmstezzjr.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gkgairzdo.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gxposlszn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gudnbowxv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gnvyrvenw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/ghauyymjl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gvlqdstce.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/ggqjlinbi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gmsnjvpvx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gdycejjmp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gkvtapzpv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gyfbstfrk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gvmscdgbk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gfinpstsg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gikcvtcxl.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gzbtmbhqt.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/giqggutdr.sHtML


<!-- 参考信息 -->