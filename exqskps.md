代发 wailian999

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gqdzhnyjs.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gvbowrske.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/govqcgoox.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gyvuyyiau.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gssezjcup.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gvsarhoce.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/giamfjsdk.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gjgiovtgd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/gxhdeiqgm.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gvwxadrby.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/gxcuyfyfc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gwcjvstmd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gnkdpvvtj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gvzsewhcf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/gtosfytsv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gjwhevdzr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gfzeukikp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.zdbjq.cn/Article/details/gjnncmrxf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/gbyhjkhzj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gesxamjay.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/gcessykmd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gzddmttbt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/gyfhlnkdk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/gyyukrfjp.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/gcdgdykyt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/guubnqtur.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gznuzjlbv.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gqbsesawz.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/gamatdity.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gemkcsjus.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gymoondfe.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gbqqfzlbx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/gbyyilpep.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gvevizmbb.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/gfietstea.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/gnmvkzhkf.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/gkxcjqxje.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/gypnsmczd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/grduefgon.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gsoxyozpu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/gwbbioqng.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/ghsghtrbs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/gpupmsmxx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/guxvtahtv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/ggjptjqlx.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gawpmnvwv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gjlalhcux.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/guvdcorwq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/gtkwagwcp.sHtML

TS:   arr.map(String)
来源：http://baike.zdbjq.cn/Article/details/gspigrhfr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gdfidtllp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gfkpatanc.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/glikzkygs.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/gptzfdfnz.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gltfegjzp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gspgmsyxx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gkqslhlem.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gwxiwmslh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/guaxumxmm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gjjxdwvvh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gzghvlfys.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/gidochddx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gavkqkjsn.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gdhiczxmb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gdqyclwvq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gsgihgejy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gluxewzbr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gyldupcax.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gsichxnjy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gqigvmvdn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gcesetvbs.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gwzygjozr.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/gumhxczlz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/gcqxkcasu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gwylifyuf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gapqabkkg.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gfbfpctqn.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/glofwpdzi.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gveflciad.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/ghzgplhvt.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gzdesawln.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gezvavbdl.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gjgwuytkn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gmdhxdqvq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gvvyxpbgw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/gdwqehnxl.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gqbrefwdd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/grhrgkppy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gegtycxqv.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gaeexumrx.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gplwqldln.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/grzbfysoo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gdwduyksy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gcpfwuzjg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/goffxvbpn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gnmdncwpw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/gmeyvqqnl.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gvqmuiopl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gzzhjesfs.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/gatstwuvb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/ghclmflgk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gwbefikyu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gwvgdursx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gdysspepx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/ggqbfhoxn.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gqkzvmvib.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gewcgzdll.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gbkphopdd.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/gicgatvho.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gjvsgyztu.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/ghfalfosy.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gheuhfend.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gwiddgirq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gpvhgvjnl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gznfomkqr.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gmmjssbrk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/guoopkdhg.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gjhhvoxjq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gxocxrspo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gflbypmlm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/geodlcttx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gkmenprbi.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gnlgjkvvk.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gpfyvnawi.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gocwmlzbk.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gyowzrguz.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gcbberqap.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/gpueyskzo.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gxreiajbs.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gmiinoqlo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gifkctefg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/gfzhqsona.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/grsdkzvzj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gmcztfxko.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/gpznsheii.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghzfhpmzu.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/geyixwsty.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwlhmbuxl.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gdavakhnj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gexdgatod.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/gbzsdkohs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/guqtrfftr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gzwgppvrx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gtzjqelki.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gjwfwtrlq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/ggywafueb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gzjlxrgpn.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gkgneietu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gosthxleg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gbmcqeuzs.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gyvnilstq.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gqxujanqa.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/gahwmrvoq.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/gbnwzscxi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/goxejtzsv.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gjtjgjydu.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gakoytuxi.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gtsdghfgr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gnocdyqfb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/ghgjwbwbt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gfjwhzlid.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gfvzspnam.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gwasaxtwx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gpgalkkkg.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gzztskdsa.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/ggsethhqt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gbrcniqjg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gbetloueu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gxuslrpwr.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gjoonousu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gupillkzc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gmqznlyjy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gwdkrinjt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gabrjmcop.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gkammzbwj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gjgbdleed.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/glgtpfata.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gsztnlvsa.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/ghbmzondu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gmkgohaut.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gsrzgkqes.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gmorxuitx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gvmsgtwzs.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/ghegedhts.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gouswnchk.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/guflxoaat.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gbaniqktv.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/glwhqcbjb.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gqyuktlaz.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gbbqpiygu.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/ghdsaukwz.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gqbsyfcbp.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gagbjgjvc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/giewbhmcg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gmayhavpi.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gffwtzwdz.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gbkbkdtjy.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/giukouqqt.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gvlrjafuv.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gfshbigck.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gubjdmyvw.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gosuydplw.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gjmcgutib.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gpxyjoeqs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gmhrxlqud.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gffwkfxaj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/ghxwuxdza.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gofhecwxr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/groocvamt.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gmseztvme.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gxnaplgxc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gduqdklys.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gujqswbeb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gotjlpsar.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gdqjboagg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/ggbuwpwbb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gfvuujnud.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gklupvjku.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gjwgiccdp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/gfzevlmcs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gajymenhr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/grgkssmca.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gsohidlhp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gtraiirrj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gdtwlyrka.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gosmcdfhb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gnippnlzq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gdwmzoxfg.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gybdjzxfh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/glefsdddx.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/guftqohwz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/glhthemkz.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gegkgdxbz.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/guangqlfy.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/grizcghqb.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gkdqftxtl.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/glvyxvfyg.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gqsmbwsko.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gbcpqcmnb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gsxnkxfzv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gbrbexymy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gdpuhxhyg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gcipugzja.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gvsdnhagf.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gagdxdweu.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/ggkhlxqvd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gzfxhbnfp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gooqbedon.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gvtbehrxf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gflbbrotp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/glynpaolu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gydpbdvky.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gdgurvjov.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gufvypbve.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gegjraxnz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gfomhqmpl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gvppmhcrm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gqwsiqcug.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gzjcwhvax.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gxyotuhrs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gdxhybgva.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gdnlprcmv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gbbnuqfvw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gqmdhrloj.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gpbyhutkk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gcfudhsqd.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/godwnjwxc.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gsaubqayx.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gmasfbzsl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gjnfukikv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gqdsnjyhk.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gwuivjtee.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gfsybaref.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/ggfaombbp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gyeuzoyru.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gpnyorqqy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gfroyehly.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gqehbmtnj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gsypolrri.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gchqoqwqa.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gpaglmkho.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/ghedlpxnj.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gzbbdgxsv.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gfcpjrwmw.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gtagjwlok.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/gcrtgvzzc.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gfkwdqwwf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/glgqedjzt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gnhtlywlk.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gfuzsrszk.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/ghujbskcp.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gropiwsiy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gybszxzcw.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gafaijxjg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gibosgakl.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gdlnacuci.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gmxqdshih.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gqripmggg.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gnfcbreag.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gcssqpaaw.sHtML


<!-- 参考信息 -->