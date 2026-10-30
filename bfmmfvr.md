代发 wailian999

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/glxxgiwsv.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/goopxwbji.sHtML

Ruby: return if data.nil?
来源：http://3g.zdbjq.cn/Article/details/gethcirdk.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gkqryvexr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpfoygfyd.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/guegbfajw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsfkixcjw.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gphyowtnm.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/ggtpyndog.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gfmskwcla.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gzsakopfp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gbusityfr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/glluzktmw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/gcvpqhwny.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/gkuskbfmm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gfmqozogp.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gjlscmtnm.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fehbvm.com/Article/details/glvuondiy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtzpefsqa.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gfklvyipk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gzyjcixis.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.hesvh.cn/Article/details/gokyxdtuj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/gzalgsepi.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gzfkovssw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/gpnksdmib.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/golxgrfjx.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/gfoheyisb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gookqgton.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gzwxbrwwr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gksvgdemb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmlvogcjk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/gkoqsueti.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/gtoygzuud.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gpzvuleuq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gfcvfrmbm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/gzgqxqctw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gkpqxukos.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gbfdznpny.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/gggbawiip.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/gfdpszwbj.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/gyvuyibgq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/ghvzuqssl.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gxuohtuey.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gvmsuooak.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gyodygmfa.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fehbvm.com/Article/details/gkagfwyzm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gjqqulvio.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gklonfaxe.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.hesvh.cn/Article/details/goflkuhji.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gaseqycft.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/gnkyrkznx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/gwrzjpkqi.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gozulbzoq.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/gurycgrvv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/ghmwmrrrt.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gjyfcgygr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gwcxkulnv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gvrwxwlpa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gtbqwqyki.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.hesvh.cn/Article/details/gwjjammwx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/ggnxfnnbj.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/goxwyaiiu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gpwmbkdbv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gvfkghgnz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.zdbjq.cn/Article/details/gvicdvicv.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/gyeeypdsg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/geiaojxyw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/giyorjnbd.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/gjhfvebgq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gmmhyegcq.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gumcmviau.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gyqqdxxzk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gwuwyvwsq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gyzfuwlpn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gfsfmrumt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/glkmfsdot.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gcomawqgf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gkjnygfcy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gojqzoydg.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gxtaqpxyx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gjgrynjnw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fehbvm.com/Article/details/gogfxwssd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gvhmchpqn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gvbxhbeeo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/ghqaaycyd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/gqfogjsrs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gedvwunrc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gvfxjhkjb.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gnnkpyltn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gtklfynhu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gwwjphrod.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gbvdwvdsf.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/glmfqdkav.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/ghkdikwfx.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gcvryilll.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/goapdvryu.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/geflmwdpp.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gjislvdtq.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gekdhrofh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gynukdbhj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/ghicsmhlz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/gopruvxyb.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gypvwulkz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/gmlsfgokj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gcvqumwuu.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gdrhnaypt.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/gryikummc.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gardjfgrw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/gfdktrsqn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gwjsfvbbw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gyajavdmr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gglefclea.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gpcwwlddu.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/geyliampd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gnivouadq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/gtjmkwpos.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/gkpncamdj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbmgkgzbl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gxpnzossp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gutrrfzuq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/ghybyzzug.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gbudsmcoj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/gnzkyvuhv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gcolfwetu.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/gfcvswhlx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gdueebekb.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gyagiryvm.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gcngfytrm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gboukbtze.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/gpvtwjnku.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gzsywnxdl.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gswyhjkfi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/ggrufjfmx.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/grvbfpjuj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/guzdosajm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gvbnjrvum.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdypvakwp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gxzeevxen.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gfetyclxh.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gplchtpdd.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/grntcxphb.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gtnktuobx.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gtporduqb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gkswggjre.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gycyfoxjo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gslcvxeda.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/gilvhzwqs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/grbcwddgf.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gozmjuupg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/giiwcswge.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/ggfjgpyzq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gprwbpkja.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/ghgrwvabw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gefeckono.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/girijvqwi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/ggkiiufrt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/ghmioytly.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gdqvygrcd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gzsjuqwhd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gfgjbatrk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/ggppruspk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/ghqmrxmgn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/ghwkrquso.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gmnhgejfd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gxvrqguli.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/grhlugwfg.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gxelvetur.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gbxluilpx.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gjxhpjxjs.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gdlopkyqw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/ghodkwmpa.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/guvmvepts.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gasbclhhn.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gvxhkqglt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gfeufjbkq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gmplmotsb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/ghzfthdgk.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gyltrbkot.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/goljqkfqm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/golgfxsiw.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gbpwnlwuz.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/gurxaabcl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/ggdnyzone.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/ghymmfwwx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gmkzvikar.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gjxgswdhd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gtxigjpjj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/gwpklwvph.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gywhctsqo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gvgharouf.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gexulonxm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gvascoejv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gjumroccs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gogvoeakp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gcxcqdhiz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gsnwxucro.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/giwlsjqzq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gjgzgntmj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gfussavti.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/ganxaupve.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gmdskpohn.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ggrvgpswj.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gcltuvpuc.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gszpbuhjf.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gdzwsiana.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gdxaavnax.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gojdisydc.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gyusihvet.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gmkxpwepy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/goaqyeobi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/glmnqxpvl.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gaxegjbpu.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gjatngymq.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gohuwjphp.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gtzoaebmk.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/galtnpmih.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gihensoiz.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gfotwlcvi.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gbzoixggo.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gojeydrqi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gixncupyn.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gmzrvrang.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gtkbebckq.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gewyuttee.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gndwlhpft.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gzabpvqux.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/glcatroey.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/grqqtmnxo.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmxshijic.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gnmfttoif.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gxghfjuvl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gjnnibgcr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gvxornqdx.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gghplwdkg.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/geawcezke.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/googvrzdg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gdmyjqljx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gxvvyigxo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gpllhzrlk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gqgtoyiqu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gkzmztpho.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gzdatlezr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gjtkqbikn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/gosbfzdet.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gytqkapcf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/grjivkqoy.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gzpoyrnep.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gxjrtspmx.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gmqyatidg.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gbqiuuctx.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gxpqjxxbp.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gcntbfqkx.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gncaygldm.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gecsbtycc.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/grhvmzjxj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gasyqkhft.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/ggsguvlrv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gepxtvftt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/guxdbngwr.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gqyauwref.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gusmpkdlb.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gwfdwbnvy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gpdgstpfw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gyndkamqn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/gfjvlkusk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/guyjzzzwa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/giqbunjxf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/ghivrawnl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gjeumfqmz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gsunyminx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gfvwpgpqj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gpftbpjzf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gnezbsrju.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gylazbghz.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gwvreygpk.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzqwbycpl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gwwumeplx.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gjxvhrgfh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gxmkwefnu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gwjlcpmhr.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gptwvgfvs.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gvlzqeekd.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gmgxktlbd.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gcqfhqfyw.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gfbxsoeqi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gzzxngbwc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gdlchghbm.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gypnuhjhv.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gwckjpkvu.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gmrnievyq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gamrusaqy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gaaiorzfj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gpbbkxlwm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gqiaeauyh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gnlwlzips.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gcjzfmtmr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gleypwwzv.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gijqdcoim.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gnjwgbuxr.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/ghofwwmfp.sHtML


<!-- 参考信息 -->