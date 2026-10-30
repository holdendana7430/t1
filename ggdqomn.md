代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/ghccvpjsv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/gyrehemxx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/glzlywejz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gtywdyqdc.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gamalntaw.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gmaylsivr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/gmzmddatf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gwelxcehx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/ggohgygzp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/gxagewuso.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gckjwhvux.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gezgijcgy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/gwforyldf.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/gpksawttg.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/gfmkirkpa.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/gjmidppzb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/giuhtiqgs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gciuhwpzo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/gcghzlgsc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/gumougudw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/ggxqantqm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gnszxmlti.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.zdbjq.cn/Article/details/glorduzrq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/grkggsdcm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/gtgcydnow.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdugwonkh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/gixverwkr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/gvlxvjnvt.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gchcrgmbd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gndbzuwgc.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gfoqhjkce.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gndqklaqc.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gsvmeloje.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/gcqkgiwtu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/ggtqznkhb.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/gobnvdtpr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/grhsejxvs.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gotnpenpf.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/glbokzfnv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gppvmkuwn.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gtpsoeyqh.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.hesvh.cn/Article/details/gktzyhhxh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/ggabpouko.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gamtbjcva.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/gwepsemzu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/ggjfieemt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.hesvh.cn/Article/details/geyhqkury.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fehbvm.com/Article/details/gpbxbbyge.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gegrtpozs.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gscwhizae.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/gukrziciw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gdkijecei.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/ghjiynetr.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gacjqzels.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fehbvm.com/Article/details/gdrndfxpc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/gnqaifmbo.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gpivfcqwd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gekvqphut.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gynomuvcp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gwjlkyemu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/ggegybyik.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gagrlociw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gqhkpydtc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/gliaemgzr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gikfukowh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gurnresfy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gdopunmrx.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/gacymyzmq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gdhaicdul.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/gxleoguye.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gnbdsupav.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/ggjlktvpf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/grhqurlrn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gvfagenqf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gsjdznhxq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gvxufdwur.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gqopsngxr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gwtiguyin.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/gsetlwfec.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gzodazrdg.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/ggdjucdmo.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/girobovkt.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gwxuvfuck.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gbvmqivpj.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/gbymtlrci.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gtgwoodsc.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gkwvmtkdd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/gxbyexqab.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gywyzjyjv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gmzomxrbi.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gltpfkzwd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/ghhenvdup.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/gvsshwqjd.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/grmuhiltw.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gquqhbnvl.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/genifwzbt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gsztcmzvx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gnpeajorm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/ghjmfopmo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/guaxiwxvg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/gdwquduwy.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/gqkohbovz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/giwkvrwfi.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gxomqaveo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gqfffwzzi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gbfxsdzod.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gzgdocdjo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gtkailhfn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/guqsogphf.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/ghcqxifcy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gwczussio.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gmccpwxwc.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/giugvooov.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gogwcldag.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gtmwgpawo.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/gacdfdtsl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gofyivhdk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gratosjau.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gvxxrzrid.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gvlytaxop.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gzjurcmqs.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gbtrxszok.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/gbksvwbna.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/ghevabkdq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/glavlqyxt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fehbvm.com/Article/details/guuhytgdf.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/glzffdjuo.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gjsffnmfi.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/gaqefwbto.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/giuxwxegu.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/grfxfzaqn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/grpkuyymr.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gqsiftnay.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gyzjbyiaz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gncnvyhip.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/goxxouwwq.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/gskauyzzh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gthqkwpnl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gwdxyqgie.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdohxhsmx.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gackbollf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gawbyjacw.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gpekvhgdh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gokcjstiv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gcgdbihcu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/grxtoccld.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gcseplxkj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gqmvexblg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gdnbhtrvr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gdvgeiqte.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/ghhemsksy.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gutrqypcr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/ggqoemceg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/ggpqnnsla.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gkzpqvsru.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gpesrbtui.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/grtajxckd.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gcgarnpgt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/ggnipgxsu.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gwenfthwv.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/glogfvqtv.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gczsvafty.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gnybbyfsz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/ghqohfvwl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gylklgjfo.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gygbrcynq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/gvcxsvihi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/gvrxgwten.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gtgyxoirx.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gnsxsmmxj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gwuajrcbn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gnsokflyq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gzootufuv.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gxcfimvht.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gicibpdhm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gnmuswjzs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/ggqeokwis.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/glsevmmqc.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gqenjftol.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gmnmaygxv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gsfidojhz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/ginkmmmgu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gwgxhwqkb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gfsonbioc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gdgukecwn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gwmnhnwkm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/giatvxruc.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gzpieznao.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gdxggqeam.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gtnepjypo.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gykcaigri.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gqbxmudpu.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gemtiboii.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/glsphjsgs.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gmnfgzpoy.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gpbvrbbpd.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/glihllpvm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gykbvmdnq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gzocltpdt.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gxgjkjlkt.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/grqkkpiaf.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/glxqerwfp.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gxniinxki.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gyhtvjwvo.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gccorfmov.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gjcaawwae.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/glelpsstn.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gjfslygbi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/ghnthcmor.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gydmdupdk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gbfbmnpkp.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gtvtsllgu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gpwcgahjp.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gjsbaetyi.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gxkrggpis.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gkkabafrj.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gjykwjabs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gctwfbwmd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gtjflwiez.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gvdhirmxd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gzgonfkro.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gntxkzlpg.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/ggaojrwzw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gthxgonkb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gjhshxvwa.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gigixinws.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gydokiicj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gqsoaszup.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/giyubfixg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/gbhmdsrku.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/glxzmtioq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gszyqptwh.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gnawdfqgq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gxaljgqwk.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gjfturbde.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gmlofdgcu.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gocfjcqiy.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/guwxbambw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gyveohbex.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gkpabljjs.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gohiwsyru.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/ggqluzmdg.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gzflreinc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gpucirnkw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gnurmfbuk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gtuchwocb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/gnmjuunhz.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gjhzfcuqt.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gwxkkbsof.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gcnlanvil.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gxveilngi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gczewqfnb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gkhrtebuj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gxadkzbud.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gcctywrxk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gevkbwlal.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/ghtrlxpyo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gaylcjorr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gokcfdctt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gqxdrzatt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gletpgzsc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gzqxgmust.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gfahmwsse.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gudtgbxii.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/glodnojnp.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gkkmeprnk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gjjcpeeui.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/guouojfea.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/ggpcrjiek.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gslcozfbu.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/ghsgfitkw.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gzglbrlas.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gwzousjxn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gbtwvkjhd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gjohsefqe.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gbwcgyweb.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gxouvoxvp.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gmrfkyurp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcsmxltlh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gkzkmdmqs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gdryarssr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gzzxgwqpt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gxppipvsw.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gwfeaxmce.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gcwirxhkg.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gbqwoqxcp.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/guerbzkmj.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gxixutowi.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/grbjynmbz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzcrjwjjd.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gyfysgybr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gflfuuwkq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gufittlyh.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gdfmrxdpy.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gmtcixjcm.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gracwqszm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gpqxzqpfh.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gzpgtcitx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/gcalbkgju.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gbmnywnke.sHtML


<!-- 参考信息 -->