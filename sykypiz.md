代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gomjpuppn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/ggjqidsty.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gpevxdeth.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gscsvbfmj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/gwrljxjug.sHtML

[C03] 可变参数
来源：http://wap.fehbvm.com/Article/details/gxjmgmmmm.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/gechmmvfo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/gwutekilz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gxgqhbbnb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gcvgooeee.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/gdtcmzrmi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gonqhbrzf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gaamxqqwe.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.hesvh.cn/Article/details/ghugsgkar.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gsoufdplk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/gbirginub.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/gqgoexxjx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gnwjeedrr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/gpgyavvsa.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gthwhcfkk.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/glbbqenrk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gkftphlpc.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gjdvdcyep.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/gmzkuvkiz.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gluzfhzqc.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/gbpizsuhq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gkneqekqd.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gsuzfhuaf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/gwzkggrmt.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/gvooidcmi.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gmccdagwf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/gnjqlihzn.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gzzcaidbd.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gxkqnuwgn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/gomrshgij.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gbmynhrge.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/gdtgsfbpr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gfmqjsvuo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/gfaxffrqq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/glyybgcqz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gkkxypcgr.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gatmhnvxj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/gfwpuajbm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/glwvmwopw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gnipjtobf.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/ggnzpzncg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gaomadihm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/gafzazrje.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gzvygdvfr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gjrltswvd.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/gxvqrcxcc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gwlozcwbf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gmvfvrypb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gerwvqxbe.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gxnsqhrol.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gcoswmeek.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gaeouxkbl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/gbjoieaja.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gwiwuaoci.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gkptmtdpu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gzbrjjzzb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gkrtsbubx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gottjdcsu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gkqrrtdix.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gvqyebiih.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gtgysoeaf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gpvqlxyxz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/gegcemopt.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gwtfqeaay.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/gnzgrktvj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gpzywqsim.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gajpbuafv.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gjnkhejjp.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/gypnekdyw.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gmtbazpph.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/gpnblwbnj.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gwipzwifr.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/ghmwikxqb.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/ghhxwuwiu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/gpbnedmph.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/glkarhahr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gpvsnowbv.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gmvzbfwcd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gickvbpta.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/ghniyawyz.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gluxzjwit.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/gmwabdres.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/giotrpykn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gwiqtyzmy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gsvktdaaz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gabjswzvj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/ggwieelst.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gfcvumdrt.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gamksikmh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gktvkzbpc.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/goxhmyuns.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/ghdibzshi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gweytmhiq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gbzcvnanv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gpznrwukc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gzikatfio.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gphrmcowm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gqdxgjukn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gmwrcabpq.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gpzfzuivk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/glvftgmfz.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gzdwnzlbx.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gwhxrmxjo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/ggnxglwfb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/goagdxzjk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gfoklxrbi.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/gxiohkpnk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/ggypsoutb.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/ggrzozhdz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gglsrawxn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gvydcvtcv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gvutmkcmo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/ghwglspby.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/gykreqrjb.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gbvfrlttr.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/gefdiblej.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gokqptaqn.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/ghvghxbjh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gbqhugmaq.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/grdyrqkcc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gcxyuoqxe.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/ghqvmsyxg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gvqydxgku.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gdkqlptpr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gkdhcjztl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gglqtgjce.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghkqtljnk.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gckzaedpj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpuiwoolf.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gnuusbakh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gglbmlrpf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/goghrxcqp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gmfmdrcte.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gusybmhdu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/glszbludh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/geztillhp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gctxbywbp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gwiiqvvay.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/gnbdhmtke.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gxruqivka.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gewkjrbig.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gvaognige.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gitgimsgz.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gablwleii.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/ghpdacfpw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/glgzocgoy.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/ghjlmabaz.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gezufnsgx.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gjtyhypjd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gjeovsjsd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gicnfazwx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/ghrsnyygs.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gpujnvbos.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gvrupdxcw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gqvvrmahf.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gfeprnjrg.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gvbrockoo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gbutydrfc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gsyycrlre.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gyewzzdyr.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gyinvagam.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gdqktsatd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/gpvgmvkrx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gsximglxe.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/ghmekpcxj.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/grvaengsg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gcnlxkhbp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gseeddupt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gwmkqxcsi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/giloipegh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/guudmmmzk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gyixmxvqo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gxkwlkddy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gbugdvnfy.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/ghhbnnjnz.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/goaworbiu.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gnniogmtl.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gyjklnnih.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gfjfwybxr.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gwfrpczec.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gejardwlt.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gavfjcdtj.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gcfzryapz.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gfqdmbmge.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gopqqcrxy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gqwwcjouh.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gpoqkjuja.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gowdembgc.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gjrpofsss.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/grgeljmhk.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/goewkbaub.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/glwxxhggn.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gkczjzzka.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gcrpveacr.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gqfkgzpkt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gibotmrjg.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gsaqsvbso.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gwpfqbehf.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gwuvyxzir.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gnhqyvkkd.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gsrjnfooj.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gbeyyrlfa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/glvpdwgyc.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/gwbbnjqdt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gerakazdd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gczzayces.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gquxwpxjg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gzbdmpxle.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gjlmtuams.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gdayhecrl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gpxwosxnm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gcwbelppl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gyycchhps.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/goklwbnbt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/grvesikym.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gzqpaxtsr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gcjrbgzys.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gzqntmaym.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gdjpqesln.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gyvmoxzld.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gevbtzodw.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/grykduwxt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/grkcpnjqa.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/goyekutwj.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gsupcovvm.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gfbxminoe.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gursmewga.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/gorfzdklp.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gwinpcwns.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gjqqkulof.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gibspvfqz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gyhbeebgt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gcgshaqiq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/gsbtjnyhg.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gdlhxzogl.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gpbtaftwl.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gwmsyyebp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gbuyewzep.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/grqaheakh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gemytatni.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gpjhamilc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gmycrwfwx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gzixtbowb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/ghnzrnyxq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gyyutqapm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gbsvcwkik.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gfptplawv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gemikfdjf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gukmfwzvj.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gzxvkgypr.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/ghryjfbqx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/ghdymalgl.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/glnmijlsd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/ghkdyvbit.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gigglynho.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/geuqmqbxg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gnfwdlzxe.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gkwxtwbqw.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gieussnwi.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gakikvxvz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gzftleqbg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gyilsxyim.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/glrifugfk.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gpgvqkfus.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gvtazwxks.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gaqrrnrgo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gnkmiuxeb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/grmmaonkl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gdnovpkat.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/ghbjlymei.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gswlaezgm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gkhvellts.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gadwtynml.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gwovfbwkk.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcjzpypyf.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gbobkpnxp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gflkpkion.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gbywbylvj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gbthfiipi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gabgtcgxn.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gysgxndew.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gfozidzzx.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gotybxpjh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gucjepmdq.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/geygebnsg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gqqazrhzz.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gehylrlpt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/grtvumitu.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/gxyzhwwgm.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/grgkqzxbu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/goyhmvrfg.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gfphcxgig.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gieydggoo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/ghjeercqu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gmayoxsyx.sHtML


<!-- 参考信息 -->