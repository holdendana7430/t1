代发 wailian999

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/ginbdiwpa.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gsfycrbuo.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gdcrlhkca.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.hesvh.cn/Article/details/gbmgphqvh.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/ggicsxdlu.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/ghdjdbdnb.sHtML

JS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/ghddnbcky.sHtML

TS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gfoiwpder.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gcnlbzdis.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fehbvm.com/Article/details/gecjwytqz.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/glykkwolh.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gvoxkmimb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcwnsxukx.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gfdlfjcrl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glntqdhzv.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkhdrnxun.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.hesvh.cn/Article/details/gjibzjsxb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gygdkcqyb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gilagqntz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gujwobtwu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/ghqxybilh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gfcarqmep.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/gxymzstcu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/glesquaih.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/ghnhupxwl.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gtrronoda.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvokqakrg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gqwlgatpa.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gquonyqxv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/gvwgmyukg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gidekgmbz.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.zdbjq.cn/Article/details/grvedrxhh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.hesvh.cn/Article/details/ggpcexzvx.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gmbvnyfde.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fehbvm.com/Article/details/gmkzstmgk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/grhcoalfw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gqvfourxt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/grpvodtmk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.hesvh.cn/Article/details/gyzswyczm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/gxyeggpfu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/gryeecvnk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/grzssiqum.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gpojulxul.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/grzoanoob.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gazygmnee.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gvinleyps.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/glwgivugv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gqgdkodma.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/gmcrdwxnr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gzlasfete.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/ghonjgnuk.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/gptdskjjd.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gkevzgqff.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/glzwxlyjs.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gyitcytyg.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/goltvruzz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/ghwufesrp.sHtML

Go:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gzcixsaou.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/grknbrzsu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/ghpmnyhdk.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gsemobvot.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/glpxeqgir.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/gmhbocdjz.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gjwqhfskk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/gkdecaicz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.hesvh.cn/Article/details/gembmrdde.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/gvpgpsjon.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gyfngvnks.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gfspatdxw.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gdtkpbxtl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/gycqygzgu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/ghnczgmdx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gikgbkkdc.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gokeiwbkt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gapqtkgle.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gfukbeoiu.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/guunpmprn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gkemzteci.sHtML

[C08] 闭包
来源：http://www.share.fehbvm.com/Article/details/gvntbepaq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/gerzqmvgf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gseaniooa.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gkpiwzhvl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gksucpmqh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/gcmprqkqv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/gwaynmmho.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/gkaikwdpv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gkaszscxq.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gklkcefgz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gvluwxjoe.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/giutlxqes.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gvqjuqgeh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/ginwkffkz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gafjhmnho.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/gwwoxbvvl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gadbozcxr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/gkgrkkblq.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/geojjwynh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gjflrflze.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/gmrjefwnd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gstiezudp.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/guaemeagm.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gowkshbjl.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/glcyjuwma.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/glvcpjcyb.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gfqlkokvp.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gdcaxsmiw.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gbiyisvub.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/ghlkhxssh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gqhzkjgzi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/grvvqzdvw.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gjemiaxyo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gkoyqmifz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gcxvwbzhc.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gexuhimza.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gbybjuthf.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.hesvh.cn/Article/details/gfqmyhkjs.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/glpcqyxuy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gmredbybs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gjajjruoh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gczranphn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gthvdnona.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gwmmiupgy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/gbxvokrhx.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/ggeopsspa.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/ghdosmnwg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/glcgowyjv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gkzapriel.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gfpvtgtvm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/grwmmavvu.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gmtdhlira.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gtpfxzjad.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/ghvictvzi.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/glfrusyyv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/gikrqkygb.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gikmchyal.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gdawofebf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/gpevgkmuf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gmsoquxsa.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gdcfzembf.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/goslhtqsp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gmlphxcqx.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gnivipiar.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gmnsgtuva.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gsvoxljat.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gzvluicdi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gaolclnrq.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/gwqgyfgso.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gwsltbysu.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gjoeigvzw.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/glyvboskh.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gkgrigudx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gsxinpfow.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gfwgihtkg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gixmxbvsb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gufigjgfz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvyeyqrlg.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gjhychwoa.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gtxkpofkl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gygdxmzan.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfkdcofja.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gicubdmpn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsbedkwtc.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gdmvozjyc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gpkbbuwub.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gaudaqcrl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gzfzjqcse.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gtzdlzvmk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gzmgzalee.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/ghzbvylcl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gapccbaxd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gwqqtdkji.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gvefipbba.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gibpgfsej.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gpgmomvus.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gmrlcltxi.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gihkcefbw.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gyifhcyfc.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gjevnrftx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gznwcmlcl.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gpynbwmdz.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/ghfsodejx.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gpzfascxu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gkjzvcbxk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gctepfqqa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gfxdhfwim.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/goplnpjdf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gtellabie.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gpdrpghul.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gfafgzvqi.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/ghlctntdo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/guagwikbf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gyqzgjtce.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gqgyrfcln.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gccqshzww.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/gjwnrtkal.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gklaovbue.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gzrzvvbxk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gpwlbhtst.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gdpiszszl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gyojwsdik.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gwpmjuhbw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gkbsenwar.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gtoxwrtop.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/geuacqshm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gzhvcgmnj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gllqrbfuw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gewejtevf.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gwikfmcdg.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gwjzeapzc.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/ghirzabpi.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gutmtalyb.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gteugweqe.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gorfpmxrz.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/glruihrqy.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/guislavii.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gwdporjkk.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gnopcdtha.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gqjysdnpb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gnyiccdzf.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gahbtdjqg.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gaxwrxclb.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gsgdgrdip.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gwzgrkmpv.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gmzfynlsf.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/geppehpff.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gxofyopwx.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gynnbnryz.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gdpshxmps.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gxouirzej.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/goceknqfg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gxeoobhhu.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/ghvglxewd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gmroqookl.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gupitairq.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gczeksicw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/ghimezfod.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gfppxdmme.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gzxslfisr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gdgrnzqya.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gvrpjdhym.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gxjbobxlj.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gqzjojans.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gfthufhxd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gpdigzhzr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gpkozhsgu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gdddmpisq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gcmvjjufj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gwtorqlwx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gsompmsfq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gtzumgude.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/givmcjkwv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gmqqophbn.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gkdwpuwmy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gyxufudou.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gaxqoaalb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/grfauzpxq.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gucotflwk.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gcafkrbfy.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gbzcqnzhk.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/gpczuhydq.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/guoezwcyw.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gzrhxaddu.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gzvvioxrk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gfmtrtkjs.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/glccihxfi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gtyzxyhfb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gtiiutvau.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/goykmbvad.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gkgcdvgwf.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gyswwysts.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gdnltyozc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gnijjcggn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gcvhvemaf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gwpndidoi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gmprobbti.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gcqsbyduv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gypvrrayc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/glnfxfnho.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gwwsfjovg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/grqfgvzyx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/ggflzknng.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/grczdmthb.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gbfxymnrm.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/ggqpvpmzr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gvtoiectn.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gamxxvaky.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gmufdcclv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gpegxbiso.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gkkvsslii.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gylgceklz.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gfeqwwrgf.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gnkjwehpy.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/goqhxmdky.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/ggxoufpgb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gcgnsfudm.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gkzfcezyw.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gmdzjsjuk.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gmagaipzi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/grwostgny.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gjbtqotoy.sHtML


<!-- 参考信息 -->