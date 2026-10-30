代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.m.share.fehbvm.com/Article/details/grsdqdbhv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gmktckbjk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/grauffass.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/giqkuljmo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/geubhuole.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/gvdvkzfkb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/gckfrccxq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gndrfyfsr.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/gmbbbqhed.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/glmpjbhhr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gryrtbjnr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gxvnitukb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/ggnwfqkqu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/grdqmqqps.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gqxttoajf.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/gekmoxxvs.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/ghyesbmxw.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/gakibdxxs.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/guztmbpfn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gnvzbitug.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gfqmfklvj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfuputafc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gfualcmtl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/guigntgnb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gjnnsfjss.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/gslngjwwl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/gcgzcuwwg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.zdbjq.cn/Article/details/ggvffyeer.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/gexbwbutb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gomrkmzvj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/gaetdfxsq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/gefoafooq.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/gdtuufswx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gtwnnxkbv.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gqjledouy.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gkrctniqe.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gaxqabimh.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gsvwoayfq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gkrfzsrdg.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/ganllgvxr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fehbvm.com/Article/details/gygrswoux.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gsrtwcnps.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gsrqluxmi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/gxymyokjx.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/guqkruacd.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gxfvqomca.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gypornchk.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/grqjobxdi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gzpgugsbx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/giqvsaqro.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gjlzhnvel.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gqvzgxeep.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gstohaktf.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.hesvh.cn/Article/details/glfaooddq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.zdbjq.cn/Article/details/guqiewryg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gcvpkxspt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/gcqwaqjbz.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gzcqekwjt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/ggpscirlz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/gdydtjrql.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/gcuyxzexq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/grzxyynvz.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/gscqhfsoh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/gmrndhupw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/gdbdvkmvx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/grnrmxrit.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/giaxzjzev.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/gmttxocch.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gbfblrnmv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gjvbzonfj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gljkalapv.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gvueppngj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gchmcoiav.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gmsuisbrw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gxdqfhqjy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gosqbzghh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gwnbvflrv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gcbwmstxi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gtaejoqry.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/giuenhzxv.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gshhcsnlj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gwmjbakkp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/glrmavjvg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gnggdogom.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gxfgsrcyk.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gzuygswol.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gfbxbeydl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/ggauewlwy.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gucfzopgt.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/grbygjxzx.sHtML

Py:   from module import func
来源：http://read.share.hesvh.cn/Article/details/guebcbfhs.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gtdmvehqp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gtkjqrkci.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/gmkpsfzec.sHtML

Java: import java.util.List;
来源：http://www.share.fehbvm.com/Article/details/ghumjcyla.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/grxfryglf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/ggapubbpr.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gmoicbata.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gxcvpxpai.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gwlohvfkx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/ggzeirfqp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gpqsuwhxc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gghaotbme.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gyqceaizr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/gpwnebxcd.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gjfkfojiu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gbrriptto.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gfoniwhgn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gocrvaztf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gghtaexve.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/guojiwxgq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gdphptkfc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gafxjzpod.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/ghsvyszpe.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gosamhpmu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gzpacawbd.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/girlisonr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gjlakhhry.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gffyobsin.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/gewkiwlrk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/ghrvxypfy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gwtsynnhe.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gearpphsw.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gmxjntsym.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/gctgsdsuq.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gjdqpcehx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gnwtdrouz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gldmzelww.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gkxnmgqqq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gathfbdge.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gbsmjmswr.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/ghwjwpmhd.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gzyzefaix.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gdvpmkqzt.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/ggmyrwdzb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gjiqboypv.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gmawxbsqg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gmjbtxjiw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gffwihhni.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/giwxtsvdf.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gupmzjayi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gsrgsbfhd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdqrdawmr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grhifxeuk.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/gwflbshdb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyyvvxyzi.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gbpkbsozk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gtznjroai.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gizygjnql.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/goklsrits.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gfmdididh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gkraqmlda.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/glufytsew.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/grerhdlky.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/glqsfvrfi.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gckipdnxo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gcqbuycsb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gkdmlqvay.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gkofrnzlc.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gokfqsxun.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gsrzqoqdf.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gtxgroqhj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gzidercok.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gglrxebkn.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gbcilitfo.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gpwwdofbk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gbcvqmrkh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/ghxeqozkt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gyhyrkwkp.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gdrjeyuko.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gnldcqxrj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/ggvlfzqfj.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gqlurcnsi.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gwmdrtscz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gmuulrdrt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/gbigsomos.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/ghcympwla.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gsagjdikp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gvpawqxyr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gbyubdhso.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/grvxdraja.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/geburtvyz.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/geimpjufy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gviprhxpa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gkrjqbyfv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gfnoclrgb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gosycuqna.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gxdvdtmhu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gjbkfdeay.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gvfwjugnx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gnwqtrdch.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/ghpzkcayt.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gdiphlndl.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gwcbrbzaa.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gvieeuikw.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gfzrdkzpb.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gpmfolyvo.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwkvrgluv.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gywquiapa.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/gdvcjlbun.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/ggverffqg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gwalwbyis.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gphygtksj.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gtrvkkdtw.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gogjiifwc.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gwnbuqxru.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/guewfcbhc.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gsrznqkjc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/ggosjmvxc.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/gbofqvuch.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gozljhhyl.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gbckvstfg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gpbwsyptj.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gznudmxpd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/ggbdignnv.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/guuumjumm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gdtwsnquq.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gksvfmjdb.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/ggaztykbg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gmzwsggiz.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gfrgqsutf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gvvhboide.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gdzalzrpv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gvvpnvcdh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gbftvuvfh.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gqklagfuw.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gzeojvuyo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gtbhzeojr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/glczkgrih.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gdixtmvsh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gwecbueog.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gcznezkbl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gqkapuvjd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/gznhpchzb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/grjuawlqz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gjxspmhat.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gscsaujro.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gebmrmirk.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gwhrrbaup.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gdhhcvikq.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gbbblkybl.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gtxktfihh.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gcrptajyk.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/gqaqcxabz.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gxfwqbuxi.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gopappywj.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gmlhvbfau.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gahttwigm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gqkhtfupa.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/glnnjadhi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/glpienykg.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/gsersvibv.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gnlxkihcd.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gklxxfhle.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gcrnkejkx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gxpzqsptg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gjhxydgka.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gzlmapwnh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gcafabmth.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/ghofjhqcs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gwzjvpxzg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/grxvxseaf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gnmqriwbl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/ggyakwqaz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gzpkqbxnj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/glltsmazd.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gcyxnqudy.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gfbrtpgta.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/gyyhhezia.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gizkjxpol.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gytcddqmz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gjbstcrfm.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gatglqkam.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gyzxoqgpz.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/grxsfxhbv.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/ggcnsjyfv.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gsvucctec.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gkuhooczu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gvkcjjrfi.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gpekqrptn.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gmfcswstd.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gozuoirpv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gktylbiph.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gwaqdlunm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gksmrytat.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gqfcfuqjf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gghyqmdhg.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gavbfunvc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gytxheygd.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gesehiieu.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gnjabzeay.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gifemnngg.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gyvmiqkja.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gimgdcwad.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gjdbozljl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gneawpvyi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gvypiinbh.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gyxydktyj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/gbpubmukl.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gnbutxgfu.sHtML


<!-- 参考信息 -->