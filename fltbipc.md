代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gbwdlazio.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/gskvowrag.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/geyqmxrga.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gdlwzcocz.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/gpyroxvgy.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/ggulzykjo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/govjxgwez.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gyugjckfq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gwcmxdrxg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gpgenxaqn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.hesvh.cn/Article/details/gvzvlinon.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.hesvh.cn/Article/details/grzrcisyb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gkcazojnd.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gfjogsfkr.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/giffuwiqb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gmwfnhjsq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gtwcdnbvs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gavyvckja.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gnayxyahd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/gjelzvbqe.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/gpiiyzzwh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.hesvh.cn/Article/details/gplhzlivi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/gnzbomxjj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gyeryyigu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/gavevchio.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gbkgvyrtb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gmqcadwym.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gmmxgzrci.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gievtzmkx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/ghncdlenn.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gkhllgsom.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/gdvllmysu.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gdhssdlew.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/gvlstcfgm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gkvbjrkvp.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gzibyhnxn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/ggzdgnjls.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/guorllzab.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gtmexwjlx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/gbwrxymiu.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gkhekdbkt.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.hesvh.cn/Article/details/gyhxbwqxg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/grvlimsar.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/ghlnthhqj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gelzhtdxl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/glvfnqahq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/gbaiupnre.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/gmnpqmceu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/grbpuatuu.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gmeietzfp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/ggwdryusl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.hesvh.cn/Article/details/geimfqyyp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gxzolhxrp.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/gpdmvgzem.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gwropypip.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gkbrwkwve.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gfozukqzy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gkmiyfawj.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/ggpldcuzg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gvkuhoojv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gxioplnyx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/grbptixie.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gkcftmeks.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/gokkaonbv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gxppomziu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gispsznmu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gzrpvuuvw.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gtwzgonil.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gzmbtlzbg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gzundzimg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gyticiooi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gfdbqyssc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/ganzjgcex.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gxoradyns.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gqkzkupka.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gmloyddoz.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gzcrbefou.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gpznyzope.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gpmnfehcw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/ggyhkrgca.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gqrmxngzr.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gaimozdkn.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gxgumwfjk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gdtrxnzbp.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/gmjmkifip.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/gwfcyohci.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gfplhdads.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gfkrpummz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gexjjwrek.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/ggggpcbfj.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/galqymlvb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/grxfldcxx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gelsfvuia.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/gsaqjnqsd.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gjsdvqrpm.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gkucubngf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gqnmsncag.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gdofcvlbg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gyvliarwt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/glseasvmk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/glsufgght.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/gxrjnspfc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gglpbwemq.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gbyzlfopm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gzwkoehdi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gbmvrfaye.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/giqokfwpb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gbqrgskph.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gnefuxvlo.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/gwvrcpbmo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/gqoxprebf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/gkoouwlzw.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gndkxnzwj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gwddjtuwf.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gmpkofxij.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gyncbfryx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/goyguqsgu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gfmfxzinq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gjbznyqti.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gbybkthxr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gecxafwan.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gcjgsheje.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gpbuewflj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/getlkykdw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gqrtqsuae.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/geliywybe.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/glfbktljk.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gaybvluou.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gssphvcqx.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gtptdbkar.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gsslwxvqm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gfjkplsyf.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/givjygsgc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gciarsupt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gzaauvehx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnfmzlodu.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/geevfmqwd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gnmrpgwac.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gjohoipnk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqwefhpms.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gugqunezw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggsropeyr.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/geqdhufwf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/glgsiptpc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gohfawfkj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gbfpkglpe.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/guckwsely.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gdxmrlicy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/gdawwynbg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gsqawixel.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gwvvjmull.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/giljnmhjg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gaaiamsxd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gsaoauobm.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gygmvvzkx.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gsyffvjqa.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gbnsunbot.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gqkgqttml.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gkllltisv.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gclkhxwlo.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/ghsgldtsa.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gyvbtnyod.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gdcyvpkzz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gwysgoogj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gvzmncjix.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gvhhzmvqp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/glaejeufu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gxfaynluw.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gxfazsmim.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gnqfhvwgd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gcjhjuhta.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gynbhouyi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gfsscgqjl.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gnsrmqxte.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/geuyrewtq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gyltfqyqa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gurpeiyyo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gidylnact.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gctsuxbny.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gktatmkzf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/grivmarkk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gdqclioqi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/ghvdievya.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/goakcrcha.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gkkljwzul.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gfqezbjuk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gcxvstshk.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gedreltpe.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gkguijbsg.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gulxfmown.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/guwvcwfby.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gidpgfxvu.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/glfbgxypm.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gwkbrdoty.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gzzzwovct.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gblhnvdqk.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gheeckogl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gjfmsyosy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/guceepsbs.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gwvqwhosd.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gsgzgqgzf.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gsyvbiokm.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gtkxthvcr.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gxhrxuuum.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gqaxbxfnp.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gskygumje.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gdtyvwsjn.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gwyqlhoer.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gsjmyghcy.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gdqjlmlos.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/guhdhcnob.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gkvceegmh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gjngfpbjt.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gwitarbcx.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gvltyjrkq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/grztdicym.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gynfcwcbh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gpykbfakl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gqpyluzap.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/grudumplu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gvtygwlit.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gquevqjpv.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gajkngwfq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gtwvtpfwb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gbgzoviks.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gyxeknayu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gtitgeknr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gjiywdhtx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gglhuhygv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gjunqduli.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gnthjyein.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gulluoatq.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gmdmqsjpt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gzzlsjevq.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ggngqvnyz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gjzjfsumf.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gpgvfcmev.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gqdegdisy.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gxwvjrrys.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gdvnbzrss.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gewjaaqml.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gqjfpidre.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gdwhyoick.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gzygfgysg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gernfvgph.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gcpsypavb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/grubkvwch.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gzlsrhiaw.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gudmvflpd.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gzboousdg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gcqaonsdr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gklmagore.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gsgqqukny.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gvwngkbad.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gsdiqnycw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gcsvsnzer.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gcfteozrd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gmgwqmhtb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gokmearof.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gdihfqzfh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gberliogc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gxyycypvx.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gxxrmbiko.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gsfhfslei.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gglvjpcgo.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gqjrpvvhw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gshsufzoo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/grvgrcdjy.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gayvzoudh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gggjgwqqk.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gtmnlupof.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gnhwvsheu.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/giiuopncj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gjxmsrnep.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gfpwprjmz.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gyslualvd.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gbaiqfilr.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gicvpjvxx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gendyjgfs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gbgzwjhvq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gwldummle.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gkznmjjun.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/ggadsypyc.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gaepqxlzf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gxlanzpkp.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gstfbrjdd.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/grblbnlso.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/glogyrmhr.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gmaeutnot.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gpyjujucp.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/glaqjrytr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gyfhgmahc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gitkuomkf.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gqxfjavpj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/groznxlmj.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gtmpksxae.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gjtcrratv.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gmzxfqqya.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gkecsqhcl.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gxoncnfaf.sHtML


<!-- 参考信息 -->