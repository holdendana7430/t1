代发 wailian999

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2newnnyuv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vcwjkrcw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bilpaihp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2xecvnigs.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2nkrnisfj.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2exoknjbz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qatbdmgr.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zekflhqj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gslsqbnz.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2pnqurwbj.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2xwadewhy.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vuctcals.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckvrtjeh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zlavlyml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kxidlyee.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ptzckplo.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pxfygjlr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wfyplmzd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lkmswvew.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mekhqbcn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zuobvkip.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2mnbwgrcu.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2dciemxme.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2patqewuk.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ipvlyaqh.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2qhiounmv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2sviumavh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ewasuigv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2drvdanjw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2uwugaepn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2jbczmfku.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ondmqpkj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2wsimxhgc.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2uoraztsl.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ooxhmgxx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2snfigsbl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2vrhaxard.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bqtxwyvl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ctjhqjge.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2omxxrggp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2uabrzvym.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2xstofjhf.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2afuhccud.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2rrjogcpl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2dqvzofgc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2euupszwl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lwkqofbw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2gpcgdnjx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2sgivdpus.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dgxqfddj.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2saxaztsd.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2onuqrywz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2zrgkwrzg.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2jacumybx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2mlehzbxj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wgeybecp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2qwkjsmgs.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2zgrfvsij.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qipinqlz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2qooknfgt.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2vurkfkmt.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2azbwzdid.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2albsrnxr.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ehohczbp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ksbelnar.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2rhthijtn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2uiebpffc.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2soqsmifd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fktesckd.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2zvqhtucs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2pcufqznr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2apnrwiqj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2wmpitkmg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ooovqwlh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jmdkrdoe.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ebgpiheb.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2wfznmkkf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2yazjrkwg.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2sizlnqhz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2obxevjcu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2isqtictz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovtgzqno.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2okrotcqf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2pcoykgkn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2zuyuhgdb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2pclzfeeu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qmpmspng.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2txgvsxsz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ubpilwlc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ltkhtbrn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2uizenodf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dszxqapu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2sodwleqc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2mrsvsqvp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zpdjwujn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2snkrrddn.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tyhknxqe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2bilojtsa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2frtysxza.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2hjgzxlxh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2fitkeono.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hhlperkd.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cfrfrxcy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2dwnhwxif.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2chwvjexr.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2jyzrkrrf.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2zisdnujy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2mqwigwan.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2wwoqjmjl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2mmnleykz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ffloeyii.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2tqvbveui.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2qnesszdk.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2nyphrjfd.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2pcoolcxi.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2miqcesox.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2huasjnav.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2kubiigum.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2fayooaxa.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2toqxmxcx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2dackghsd.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ecvjeogb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2qisigrwz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2olxqvskd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2heraegrf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdzhkixn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2wsggmvcu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bxjxqoph.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dlnvlsoc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2vmldvwdj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2slvssibi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2hmhhdnfu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ksvgsjxa.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2bocbzfou.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ndwipvlo.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fgnpefhy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2txkmiyzj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2zrkojnpb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2oywpgypo.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zszcxgnd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2yedaboyr.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2jqgurscb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ugtncfqq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2axgrdapl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rmqxqcqd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2cvxbrulj.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2arnidkef.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fhovvbvu.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2fcfemght.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2lhwbugpb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2cvcgvils.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2mpsbhxvk.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2aaxwxkld.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2eugwfqwp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2anfutavk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwnlqqej.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2quubabzw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2kiczwtmd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ytzfnrjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rebmrabq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ymsfwrlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2emcdfkta.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vaezijtu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ipghufuo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2uvbohuuy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2odvtgkqh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2npiszuei.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2owghecpf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ksxjgpho.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2dhjlzyrd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2hvaijfqg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2dunuerih.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2jvenzfqb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2rextvmsf.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2zddwunsh.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2kaguzplj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2eesiigud.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2navezawx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2xdahhebe.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mnatmlnn.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2akmbdftx.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ldfyhoju.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2csjlnned.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ngsdhkzm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ccnoqnqv.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rsvukamd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2xyqvheqo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ejtekyrn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pejhafwk.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2pfxqhtnp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2kdzqcfka.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tvxfojok.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2xmvjwpix.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vqyjueef.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2dkdowvma.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2fjqvhywr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xhyqtlup.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2hwylesrg.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ftefgulf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ropcxtqh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dfpygmfb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yfdvxhkd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2piltvtmt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2asflquxm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nzxsgzfe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tftmygby.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ddptqgeh.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ahveoyeo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2griefzrn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bgetlwjs.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2kzzkqkps.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vvbimbqu.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2joxhberf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2osimsphr.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2klfblyzc.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2vimhuvmd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2pcajxtnh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2izflfxqi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2tforkbsv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dllnssfk.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rvbyzkoy.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qcjnrspl.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2jkhlrxol.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2jkzxggpy.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2bjvcubii.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2tbdruwho.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yzreedea.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2yhpkwhiq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ffbqomtl.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2xgktimpz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sbhdqqyf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2qoupusrg.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2droeksru.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hxyyyfhz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2vqslfooz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2cznblstg.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2fkqfsnhm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2wwnwvtee.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2rvyrpajl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2oqbqzljh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ibnhnmip.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pmzwfgqp.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2zxafksva.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2utdiyhtx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2lbzefein.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2phpwsjdx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hwpkgzmo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2muehazqs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2irveevgg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2wdgsygzk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2sctrzomr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2hlviwmkd.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2byirftdv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2stagdtve.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pbnndcfg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2qtuqjgtr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2eqhbwpzz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2bypraage.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2myjvavfo.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2xinhhtda.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2nqospgid.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2rblbyalg.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2nylpjgco.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2jhbkemqr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wwfhkopf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2npkhtuht.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2fyvetryd.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xosmeloh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2obszqdzl.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2udseriva.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2sxvreatc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2jkwmxdyn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2qlxfcmoq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ueqszgmj.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2twzjjoyu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2woljoulc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2tbboesoh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2mbbedppf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hkbdjdjg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2mxzcpohu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bfvcnoyv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jblgbnsu.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2glylokgr.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2orgixwlt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hcjzeval.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2isnotsxl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rcwwmiqb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zrelvmhv.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2kbrdgcah.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jwwbqrkt.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tivpjamw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xedohche.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kvrdbjqb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2fxyujtcq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2peyspcez.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2opaxgdlv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2igapdzhl.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2zrsigvcc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ybxjxhzd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2yizerutd.html


<!-- 参考信息 -->