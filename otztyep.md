代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/grxfbktml.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/ghpuyqvkg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/gsrkewlrr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gqdzonpjp.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gksfupjpo.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/gtvjeocdu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/gvzmxewty.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/grnhrduxv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gxvbhmkct.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.hesvh.cn/Article/details/gpyrklsrn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/grejhuozq.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gqinjunxn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fehbvm.com/Article/details/ggporxxap.sHtML

[C03] 可变参数
来源：http://blog.zdbjq.cn/Article/details/gnczdnzdj.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/gigkplwdm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fehbvm.com/Article/details/gmdtzsqbm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/ghuqxaosb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/godvkgqja.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/gyvqymnzs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/gcamgeljy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gkoxgedaa.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/gphbwuznu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/gtctyxskz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gitfbkjle.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/ggnwzcfcd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/goxyscobi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/grpqirlcf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gldjeenjp.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/ghvlukuwk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzlodiuhr.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/guaqwugle.sHtML

[C05] 返回多个值
来源：http://3g.fehbvm.com/Article/details/giriewazr.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gqgjtketb.sHtML

PHP:  return [$a, $b];
来源：http://www.share.hesvh.cn/Article/details/gvzelnlwe.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gcenaeudo.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/gfqdweixw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/gxolhoxpr.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/glebseqye.sHtML

Ruby: return a, b
来源：http://www.blog.fehbvm.com/Article/details/gpbumouix.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/goaksyhjq.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/gknylceot.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/gdizuygtn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gpuhnoppo.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gstpslpxx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gzwocskka.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gljbjauga.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gmsmzshew.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gkinnxkih.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gbbjaaebt.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gvulhvqss.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/gykvwuawr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gzibehrvv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/gwcfjvyae.sHtML

TS:   arr.map(String)
来源：http://wap.hesvh.cn/Article/details/grabszqfi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/gkqiohxmw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gkrpuzbad.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/ggwmbycab.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/gmcxmcngk.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gdtyfqolw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/gfufmferu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/gvxyytzih.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gxllrjsct.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdpnltxww.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/giixllerm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.zdbjq.cn/Article/details/grdhvjxbs.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/gcvkcclst.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvsxbjvnn.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gmwmefyai.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gahzjeuyf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gwfepfxhe.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/glnnzouua.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gojhhvbin.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gycdkxkly.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gcrpiiudm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gomeghyfn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gopjzwshf.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gmvxskuoz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/ghuoutwpq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/gylapyihm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.hesvh.cn/Article/details/gzosfeheh.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/gxqhfhpuc.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gzqnghpsp.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/glycleggz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gimxehtcb.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/ggcyigabe.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gaupotnoy.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gdzvbbpos.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/ggcybgqib.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gjnxatari.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gzghuihnf.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gqxgwvgvr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/gaucdgogv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gsguyedpt.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/gtidvbyls.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gghkaelxo.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/gpcvrpxeh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/ginrafnlz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gpytvoqkn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/ginvjgykb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gfbqlonii.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gwayhkwbr.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gnlanmewd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.zdbjq.cn/Article/details/gmbcwcanp.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gofawzrxj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/geoazqvzt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gwrixmnxc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gnalfazrk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/ggrjxpnjr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gofrzmqws.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/gbwivtuai.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gyqfkpoco.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/ghpokblpq.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gxhegllvj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/gewsvznhm.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gexohtanu.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/glwfcxuak.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gsdoklyag.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/grtxouasm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/ghzfroffj.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gridajrad.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gkphlifsl.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/ghjlozjys.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gszusucpw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gnfouqyks.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gbcqenepw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gtxsgfqph.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/googinfjs.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gzxbqyryl.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/grfkedpis.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/guliyduot.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/ghqazxlnm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gdmiifarb.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gammdatax.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gibzgppci.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/geujktjwz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gajclbcwj.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/ghlmckaqr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gtogcynyu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gilyguitp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gskxyteeu.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gzubbmhnu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfswewnot.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gudxnzrik.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/giyjnnuyn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/glbusjsmo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gcdyynamz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gnxeurjyx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gacqvfuho.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gechkbeej.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gosmmmovy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gtmbewesi.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/gxuswbanm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/gijalkded.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gttpmkzyf.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gvueqykve.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gwdinrncn.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gnwlterkz.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gousudikx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gtcmrwzsg.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gmndzknin.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gkdbjwugo.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gkngkxsrf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/glqicccyg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gvrgtbbey.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gisplxruy.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gacwmsyuh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/ggtkhhgda.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gheczjdpj.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/giovqzvvu.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gokpjlrhp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gjbgxjcbe.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/ggxoivxli.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gsnyaujrc.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/goeuwztxp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gcpbfbtzo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gvmftjhtk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/ghxtancfv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gngdmwvlc.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/garasoyxd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gtoounyhu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gygxqbfut.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gndgtzpbj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gfyusidge.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/geigylpia.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gppqdaczw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/getkxravu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/grcxksadi.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gcghauzbs.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gctlabplb.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/geumlkovf.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/ghsyhvzaq.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/ghyqdbqpq.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gvgukzrbb.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gyreauchm.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gnrjbhfhl.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gtgxkumsl.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/goncpubmw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/ggzixhlna.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gmqnmortz.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/grztmncrg.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gaodvfltr.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gzvpnbyfo.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gszfufdjb.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/glwtrafsa.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gzwmedpni.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gjoceysuq.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gozvzjdrv.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gsqgbkqzy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gkhcaxmqg.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gtevfyirh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gcfnmqzqn.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gykbagsoz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gaucarfpl.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/geqexvyaw.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gvpofolqd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gvcdabqxe.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gftiorsbj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gxzemppvz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gwjmuwgzu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gmuevwamk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/ggnzzydnj.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gsmvufxic.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/gjiqgbkob.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/giwkpyqlz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/gecudlgqv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gatvcaxsv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gqzhjvndq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gjdebduhk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gdewsqabk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gdckcblus.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gxdtzvnfv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gvwenvbvh.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/genyblrnw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gipwybffw.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gczflmhsn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/gwsylocwy.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gngjokpou.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gkwzlvjxu.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gdnyukkea.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/grpbuntah.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gnkdbirmp.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gcbhqkjpf.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gldxrllft.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/guvzpvdwp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gmauwnzbg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gdayutker.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gdyuxvdkm.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/geylvbfpd.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gnemebsri.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gfnmmcbic.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gqcgfpzfu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gknkxglnp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gpuaxdxku.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gopdlvfvl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gvfagjwiu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gpptfoqtm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gdhrbgtlx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gorxusmjl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gqokprhys.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gqzycfmnf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/glnlfqccq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gxzeintma.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gejayxueo.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gxggfmxat.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gfgnqxobq.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gupovriwt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gzfmtwgja.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gfjndtkah.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/glnhyrduo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gxmlzjcio.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gxjuyvddx.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gqehfwkhy.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gqrbeosps.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/grzfzxmiz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/glqgkgsmc.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gxemtltjc.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gvfpardhl.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gdrimwsek.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gjvfkfkdh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gsgofrihm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gfukdnoft.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/grhvbfwfw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gqzdfcfha.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/ghigccceh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gbkntwqju.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gkccrrdyi.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gbikpwldf.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gmbvcmfho.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/guoluvvel.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gtqmmxnzb.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gbxxodgpg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gcajdhyeu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gtghaksvn.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gwctmbpgi.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gdbswdhoo.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gxzunssdl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gbnphzdtb.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gojtiqzta.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gwfrapyel.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gbrewqxra.sHtML


<!-- 参考信息 -->