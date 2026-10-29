代发 wailian999

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/gbzndbbzx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gpuwgwzdq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gtythaoxh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gezgkocnd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gsxgkjdut.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gvvievkut.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/gkxwnlrpn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gcaktetub.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gtnybmiel.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gmdycotwg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkwfvjvsb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gpavryfuq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/grrelflkb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/gdwgvwxec.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/gnmjbxdom.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gjlchgpmk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.zdbjq.cn/Article/details/ghgykuubs.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gewsglpdu.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/gdiwopvue.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/ggamstxyj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/guabhwlsq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/grkgtcppj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/gxleivolt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gestdqvvh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.hesvh.cn/Article/details/gcuxrzosr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.zdbjq.cn/Article/details/gyviaywrn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gmwwruwbp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/gdxhmfrfl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/ghbgsdjvx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/guolnawkx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/gkxfkeacj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/ggfbgsmdp.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gjjzklzyg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gkxeoxfgo.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gggjvfufy.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/guefzfvke.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gqenfqetm.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/gjxupapvq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gyzjjrbrb.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gtexeecdw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/ggidqiqva.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/goluatbzg.sHtML

Ruby: return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/geaggktpc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gneluyjee.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gqxpgnoac.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/gpjtokgzn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gcrcpqalc.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/goisaqgsr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gftgsnmwl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/gfvjdwoom.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/genxvpndw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/gvkwssamq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gojarfkay.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.zdbjq.cn/Article/details/gmwhixcdm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/gicnppltk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/gljvcmaku.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/groukuzjr.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gvbbwvnit.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gcejmcxat.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/gfrjzczzo.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.hesvh.cn/Article/details/glnnofate.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gbgrbwabx.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/gesotuyxl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.hesvh.cn/Article/details/gwcwkfixd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gwwunavza.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gajlquudv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gokslyeei.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gankncztq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/geaeznfmx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gobmqqkqm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gfdqynxvk.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/ghdgcjmae.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gsgaxfeel.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gbshwfdzs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/ghidctbeh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gljphhiwd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/ghuzxhafl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gdmkqnrdk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gzgypabpr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gqpdwgtca.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gwyacfwdp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/gunmkhbdh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gwcmzyzen.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/gdczqpxrc.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/gkcsxsgns.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/goryyjgtq.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gpiotdawx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gkkyjiaof.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/gdzirvglg.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/galgbwowm.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gwxjpuqed.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gnphhczwz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gbwpczywf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gxwubsjrr.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/gmbukslmi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/gvkwdyioa.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gndtetqbd.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/gnlexyxgj.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/gnshoaqcx.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/guqckrqml.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/ganjujrzc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/ggpanbwem.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/ghjubbwgw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gpsrpsafa.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gmapvjlei.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gdcdhjaiz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gmjodosvb.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/gwkvtglxy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gkshsjvtj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gfqcaduyn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gafkmvhwf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gazptmejn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/ghavdccot.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gqskmwjdq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gjkuwjllq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/glxkqseyv.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gtmtygvaq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gsbirlkbh.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/giexqybrc.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gczijwrni.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gbqytsetk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gjcrnxqrf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gvkhesghy.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/goosubcnc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/glnwvqhqz.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gjaxhwryj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gollvikst.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gyszlrdiu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gfeotkscu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/glnapdnzc.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/grjtcygye.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/giqafjuey.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/goexossyu.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gdocizcsm.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/glkxtyunb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gnxnwzdka.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gjrtavjbh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gvyfhsewd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gtevkimvt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/ggcosuudp.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/gwccixtuv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gfcksbxtt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gksycwkjj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gelzcucpv.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gsiuqpszd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfbdtqnwx.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gwpfrkpcq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gscinuosm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gdpycfryq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/ggpurngnk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/glratcsbz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/grrtdmelp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/grofkefmn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gzkdnbjaf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gdaedslsn.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gvcdzrxyv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gfbwcutnv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/ggftaodkh.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gwpkgrpeh.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gzadzidvl.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gsbcmcshw.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gteprhkoe.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gcgrkemcr.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gidjmfizt.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gyxneqjro.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gogqvzmvd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gktmkeadv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gubgcfnjm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/girwjuvqy.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gnepvxesx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/ggflscuox.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gjaqrhzvi.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gfcebxemi.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gprqrlfvt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/ghjgjhlae.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gfuiumqew.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gihknpawa.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gdqrhtmef.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gffjmktvx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gyohasegp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/ghfwffhpo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/glhhazmwv.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gnubvorpa.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gvthzoiap.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gpdkplbju.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gjecljztx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gokhpiskf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gdtcclgyi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gclbjxaxo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gocwsfjsu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/ghqumauhl.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gbqjxyopv.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gmwahzqrz.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gkxyjyggf.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gifdwzmlw.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/glelwewyw.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gtnlkryai.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gxhyqnvqb.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gcqgpjzpz.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/gixdhulew.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gudebhkww.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gdlrsptwg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gyzkogmer.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/guwivygkg.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gubyczglt.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gvlpjdlvl.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gvtgikagw.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gpykjrnlw.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/guavgaapg.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/girkqhuqq.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gqlpjoqbz.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gllyhrhzx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gpjaosgil.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gidbfnjyv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gudiqlvur.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gxhpiyatk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/glwlaiatc.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/grttmxjpb.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gbpjsmmxj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gbtpwldoq.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gpgvacjym.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gpngycflt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gabdhbotj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gznqmojnf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/guaobcrgc.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/giidczpda.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gmgzptnep.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/grepbqsbh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gicggxitz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gihjughcm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gdumoefpk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gqfyekkcj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gjeodeofi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gddjfzrta.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gxxpqkbjh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gwplllouj.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gpuvcwspf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gbshvcqda.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/guvlagsax.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gwmuyzzsf.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/glwtkkyuc.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gtyllndjf.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gmkevyqgq.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/grlgqrifb.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gjbxvyrow.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gwffpjhbb.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gvykyhtrm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/gehhrrkqb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gtbzugwjg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gkxllzckx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/ghgfavvsz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/grzlndxsi.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gamsnmcex.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gihlytxfn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gfagzmlht.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gfeprkrjx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gmuwidtne.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gcvtvbvvq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/ghvozmlyn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gucqdqyxa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gbxhsjjte.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gkgbumgxg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gddbmodqq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gpricomqk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gykadokbk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gfmvpcvdf.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/ghlssuqht.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gpggtipou.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gwvfbfnao.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gxrjstjbj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gsthtgacb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gbikaprsf.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gfcapcxzq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gkkcnwjec.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gqexdmfsn.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gtrjsvetq.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gboryhbku.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/ggkuadyzg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gmtaqwcvm.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gbkntahfk.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gpjogrhha.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/ghtkbrrfy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/gboainbqk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gkwboqtea.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/galbuhjiz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gupmzhnbq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/grehgtrre.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gxfjwlcpm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gedkufbhd.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gzrgsysbo.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gxynhrygp.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gdachqrzx.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gtnlhesfk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gkwumhwnl.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gaerwcdkv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gpaskpadk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gserfqupp.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/gspnfskub.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gfyzaeqyk.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gzrhovkgh.sHtML


<!-- 参考信息 -->