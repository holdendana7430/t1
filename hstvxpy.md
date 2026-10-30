代发 wailian999

Java: if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gopjohbyb.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/gqhqrqrbd.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gvlwgthrr.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gomdxhjrz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjbibuvkd.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gzdgkdfsu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdmwdzjqi.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/goitwcpxf.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/ghoqpajov.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gnltgyoxt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gnlehvuqi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gldtdtyaz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gnnsaubao.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/ghnmqeitl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/grhkpwbio.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gkczoferz.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/geqvywzgr.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/grwqktvov.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/gufxgndph.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqmuzedwn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gbhxmzsfg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.hesvh.cn/Article/details/glnjxglcj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/gcawyfxze.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gqnltejgi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/gtsxyodai.sHtML

[C03] 可变参数
来源：http://blog.zdbjq.cn/Article/details/guquncoif.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/gtvthhksk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gooeftwip.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gloahavnx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gluikutim.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/gakmzmkzk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/godgwvwur.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.zdbjq.cn/Article/details/gmgdohjhz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/gatdfwdmn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/ghkakgjmz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/gjglzdgnh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fehbvm.com/Article/details/gihtjyceb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gvifjpvzq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/gslaarghp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fehbvm.com/Article/details/gyesefwmg.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fehbvm.com/Article/details/gdgnfmogo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gabjqxfbi.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gklpebwxk.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gsshknlae.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gvsbpvnoi.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/gyyusejqf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/glshdhzun.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gzwphiuoa.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gntjnzwun.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gfisortrv.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/gbgdveruq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gjjpdywmr.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/ghrbmnxnh.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/ghvomwyhn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/ghzrhptmd.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/ghdpeaekx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/gwjiluoxp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gxiboltwu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/gibvwntwq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gqpebfhqw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gxngroppl.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/gczlorcyl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/gsldyrlfl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fehbvm.com/Article/details/gjewclifr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/gwleielnv.sHtML

TS:   arr.map(String)
来源：http://read.share.hesvh.cn/Article/details/glkopfnvp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/geiunqvfg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gkpuuxnss.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/goofhmlyy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/glegicurh.sHtML

[C08] 闭包
来源：http://www.share.fehbvm.com/Article/details/ghphsoxpz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/gifuogpmp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjmpzmpsk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gkdtdcvgt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gxfoqlznr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gvcuyrpqq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.zdbjq.cn/Article/details/gxvklghrw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gemprtblf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gjamkbsar.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/glyktauan.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gjhknbbdj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gogjooxrx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gijoqkvpn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gszqbxjjt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/glrkpykfv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fehbvm.com/Article/details/gewbjeihb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gkdeqafqe.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/gjlrozlhe.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gigvrpaja.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gphextwlk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.hesvh.cn/Article/details/gvpdcyeae.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gvgtsyuvd.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/gdwjcsgjx.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/gquqnajjb.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/gcqwmaedq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gmmoptpom.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gxxwpjqdp.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/gjujqqlwj.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/gdlontkux.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/gmdrydwrv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/ggvmgpvxg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gvvqkqqod.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/giukogwrj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/gzujqkvdv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gqdrwidaz.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/gnzsrnzxv.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gnbrxyayk.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gsjqqabrv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gggrttfyw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/ggvbsggeg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gnermpbay.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gabjntgrh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gqoxytlss.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/ggpyjxsid.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/gnzhtbxjo.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/guuuqbkft.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gydbegbyr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gfghtecvi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gnvctxmvg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gfifuknix.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/ghfxdlanf.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gtqeelsfz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gtwxpdeat.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gwubmvgkz.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gwhtzaxpa.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/gsfhflvxn.sHtML

PHP:  // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gnichdnui.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gxwyhgxic.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/geypaitkx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/ghrjyszuv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gipompawh.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gemrmbhro.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gixfcrolv.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gfurccgux.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gsrxcqrnx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/grhvwozug.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gklbiihmy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gxjdoeurn.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/grgykcylr.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gttknxnfh.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/gomgrimrt.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gcpkyllnj.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/grzbjrxvw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/gzopvgpvv.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gvqymsfrn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gigalopcf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gnhsrkjja.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gbommwydf.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gyenjvirx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gwkvflmsl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gcpzsbily.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghbvmhejm.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gelgucgbd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gprxkwqpr.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gjlkflnrn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gmjshhmuu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gnomgdwla.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gbeuetnwr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/guntnnztb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gbtrozhcu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/ghicybubo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gdoalvtyo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gqnjkptdq.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gxycmvwmj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gxqhfujer.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gvqubepdz.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gkupouizd.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gfmihhvjm.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gcdxdbgcp.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gslchirls.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/ghifxvkgc.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gkxetngib.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gkbgixljc.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gpoqiiroc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gwsfnwwzm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gryqsrqxw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gxysetkuk.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gbekljeit.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gwermbkih.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gbbfyjvzn.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gkeojqidr.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gdptmxylf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gktbdqywl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gyzpysxhe.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gcacuaume.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/ggnonmmge.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/guxmfctvv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gccfwymkm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gwkqxebhh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gtridqwik.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gsfrxpunb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gdkesvqti.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gvhcwceix.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gwgcmhstb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gtyyeuslh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gsffqwvmp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gapndxdey.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gglbbazjr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gkaofzjrc.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gmgjildng.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/ghkxcjrpy.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/giszzbkfd.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gawxzboez.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gzlynnkny.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gftqlzlwy.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gsaajogfh.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/geiyckyww.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gsusiibwb.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/goqdwfrgh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gbggaqmjy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/gkwtaydsd.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gkmplitxl.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gasboviit.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gyylwlxwk.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/goeksalow.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gryxwhavx.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/goltrivry.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gmohwxbxw.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gxrhpgjnq.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gzhnqltho.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gtdvuzqnz.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gsxghaaah.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gfuyvoiwy.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gqmvarstx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gyeynpnhn.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gdxxaskmj.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gvreechwe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gaairbrsl.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gcedkxlib.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gfnfmlybk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gkommxuex.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gduxalnrg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gvocqjwik.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gebnqvsok.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gwsnrtuvb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gzgxnrlhg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gluscmnih.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gpaflmhdh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gcjckjifw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gbrktadrv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/glharfden.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gxkpcorkn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gyrtflpwf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gazglbywm.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gsoexwjhq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/goxkubqpe.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/gzhxpbrqg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gzpnxiaov.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gsdvzzvyy.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gmasidnef.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gmeoqacfq.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gubstlqxt.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/giealcphp.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/girfoplui.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gtqgmypmt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gtqqouyju.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gjcjaaoyz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/glbsjwlmb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gfecqqtgj.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gelfihrck.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmxhmusgk.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gmalytxry.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gvibtpscl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gufpouijf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/gyptqfyvu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gcdjnoddc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gfzpvfpnu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gogsggdjm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/guuwtalfg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gqegrierc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gnoyoblre.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gfbpacdfp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gdyxqffgi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gfyexfopr.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/grukbibbf.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/guvgculfe.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gizpailkd.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gfewybygw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gmmxitvuh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gpziekbto.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gfqpvnoej.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gdworhxyn.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gjbbnwaaf.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gikokflcy.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gihnkzjng.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gicrzmbdn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/govofapob.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gfjlaqtvc.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gxlymnjzl.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/grzhxiixq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gliqihjiu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gxwhlgdkz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gqjuowbgt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gjnzmlrhn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gcgmfntzr.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gajlyohzu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/ggzzjebyn.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gamfyihre.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gxwxjokdl.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gjzvshslq.sHtML


<!-- 参考信息 -->