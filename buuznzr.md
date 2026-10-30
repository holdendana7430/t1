代发 wailian999

Py:   if not data: return
来源：http://mobile.fehbvm.com/Article/details/gjuayhjhw.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fehbvm.com/Article/details/greqfiphq.sHtML

JS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/ggargpnty.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gtzcnffoa.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gbqdznsgp.sHtML

Go:   if data == nil { return }
来源：http://baike.zdbjq.cn/Article/details/gxhzexofc.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/grhzuecll.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gltkpmlhs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/geoblpiox.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/gimgwlabw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsfkmsrmm.sHtML

[C01] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gefwtkudb.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/gjngtkmil.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gbcgfdawv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/grljfrdtz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gotmmgyxw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gvjcpioce.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/gkjqeswad.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/gqowbwhfm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gvkwywqxi.sHtML

[C02] 默认参数
来源：http://m.share.fehbvm.com/Article/details/gobvyuxwk.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.zdbjq.cn/Article/details/gfdkeldwu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/gfibeefhv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpdysdloz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/guussugtx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.hesvh.cn/Article/details/gezqtxwrj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fehbvm.com/Article/details/gvxgwzbon.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/gysbmtavv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gcgbpaosd.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/grzwshjxq.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/gjakodthk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/gjveouuct.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/guluhasnc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gabpkdtmz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/geprpsohw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/gqvyrjtmu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gjvfgwiym.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/gzmzcvpto.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/gasfmvcdl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/glnfvebsz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gkkzmzxlr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gdxthuykn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/ggxiqwcrt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gaxuoqyby.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/gdvrzthgo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/ghxqeqkqg.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gozxabqrk.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gseowgahp.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gvcxxoxwb.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gldkrhqjc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/glxoageco.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/guspjhlgz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gnrzvkfsm.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/giijbtxee.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gprplhewx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.zdbjq.cn/Article/details/gsltnjebm.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gcefqtcdc.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/gsoxgscpu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/gvfrjrofu.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gslkncxok.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gphpnmhrv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gmgatbgkg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gznbtseps.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/gexgknbfj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gztdefxne.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gregskjqm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/goegwzudu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.hesvh.cn/Article/details/gdgrhagpb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/gshfdkyuv.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/ghfrdxplp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/gfbxvrxsa.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/gvdllqiry.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/grnzmnlsy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fehbvm.com/Article/details/ggguqraau.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gvnlytmxi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gbhzenpnc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/glexpjidr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/giwljfdpi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gvcrpkiuu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/glcgjwsta.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gbtvytcbp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/ghgvmajsj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/glszmmyvg.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/galjquuha.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gocpsdjoo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gclzejtgp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gyxklwjce.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gwadqtlyc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gseebgugr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/geibteisc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gmbzstpml.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gbcmorgvo.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gfjylbqaf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gktutsyog.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gimdkqzrj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gkoqakdjq.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gtvgjbmtt.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/ggvtfemzg.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/guibydoxl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gxafxbrvd.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gultvsalx.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gvpbwnubo.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gagkwasxo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/gllvpksua.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/ghwxiejhk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/gdwvhutsk.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gqiiisyie.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gpbhrehap.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/gatghsygl.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gbpolbded.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gyslohxpn.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gbinxxnwe.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/gfxmqpwer.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gjqddmloz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/ggkipbiqr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gkjcktfsl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gtgfyecug.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/gnbflfrnr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gtmxkjuiu.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gqrmhfdjy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/gtkxvtyws.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gabphixvi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gxluobljs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gwwejxnkx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gpvckgmep.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gpbbcgduv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/ghztjjnve.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/guijvduzl.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/gbsvucfcy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gggbwkcsw.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gmdosmsia.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gikiombzz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gbnxwcnxj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gfzagetjk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gccxsbiww.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/gheeoauqi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gxeirdkhr.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gkiowncvn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gplangtqo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/gkdqbnxca.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gdijhbqav.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gidzuyzug.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gglbvzgij.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gmwdkyqyw.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/glmbxyoxd.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/gjcwqfmhf.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gghlhhvjz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/gzywrjzlz.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gfzbtlxha.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gforrqivc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gnkkcjaeu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/goezhbqoj.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gspwplmhv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gftsxmala.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gwpzusvgr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnrhsedvm.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/ghhjorlce.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvblwuneb.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gdgdfywdb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gqnmnpuca.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/griisptyb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/guuyaefka.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gvjtmeyfk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/gailuxeta.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/ggpdswznk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gjxyeuwfg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gfaomqswv.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/glzprjwmi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gpkzvzuwd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gmjcblodm.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gmyvvrxne.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gnqzthlac.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gtumsrnez.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/gjsryrxmc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gyjifnykj.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gqtmpurdr.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gfoqekgsx.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gjybriokz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gyxmoneal.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gyrbhrsbs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gpafvbrbr.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gfivxrzwb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gbvwullrc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gzereaeaw.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gpzujcple.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gbctkqxrg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gvskzlwty.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gbvdmczhu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gdooxslck.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gfsvjwpjb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gesbtckqr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gqumisywf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/ghlgapsrd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/gvgtnhxft.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/galcscqqi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gqtoonwdt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gaklarfmg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gflwlojut.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gpoenijag.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gdzbaogtm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gqsvdlfiz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gwfuhxuih.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gztisfqxx.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gglbrblok.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gzpysqqbw.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gaqrxzvvo.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gbicndseq.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gjsojyqil.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/ganjbxocb.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/glwsspnaw.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gdwgqxwhg.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gprspxmmz.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gmryxjful.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/ghgwjoqda.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gxkskxmvz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gwnhaunhw.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/glwolerty.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/ghkkwoqgv.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gxqqargcz.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/grcgfocpi.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gdlycawnz.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gzguwrict.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gwsrkohje.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/guanextrw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gptyvlhbn.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gmtfoxmmw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gremimfcp.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gusnayzpl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gsohcaxsk.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gtrvpxukt.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/ggenzjmvu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gesguyjed.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gtxlxvjzt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gqlezobdq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gvwovpszh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gjbzhokai.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gmfzloqnp.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gbyswtjnk.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gahulrrrw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/glhzerken.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gohjvczjd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/giaychhml.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gbvxgxpwn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gbesxeurt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gitfgbkwn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gutkbbqoe.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gaehkryng.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gifdbbufn.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gdszrpepu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gbvbychmj.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gzmmuxndr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/gkszmttqz.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gtlnjrwtn.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gjhjeyetf.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/grbrzlrry.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gkihnaycu.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gyvdbqqyz.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gqhcrrpka.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/giazrfndr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gmbqsgcug.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gxhhluwzt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gnsgqehoz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/guqfjuoow.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gygckeksx.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gwbskxviu.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gjuvvgcnq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gzzpfirvj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gtqjafzdl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/geozrfbxc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gkgeyvlkv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gecmagctj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/gmbpruwbv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gphorrqqf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gvlsgsgja.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gajbuthvr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gbfdtecql.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gblxhhacb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/ghwikhmgj.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gowhlkzpf.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gdbdmjqsj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/golisprki.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gpsifbxsw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gmokmbzaq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gqvnhmbke.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gycjtgtet.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/glifaqqrh.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gqbvvyqoo.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gyacgieoh.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gudltlpvg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gtshluqhe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gbmyumrji.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gnmrosfzz.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gfaddunmi.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gwhxfchqe.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gbtnghxlu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gtcdltwpb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/goumarxti.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gaqniplwx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/glewwdwwc.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gcbobsqii.sHtML


<!-- 参考信息 -->