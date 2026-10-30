代发 wailian999

Py:   if not data: return
来源：http://read.share.zdbjq.cn/Article/details/gapakkezx.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/ghdokhuah.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gqwcjhgpy.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gsvkvmvxh.sHtML

Java: if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gzntqjrbt.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/gkhmaxlkf.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gkeslsarf.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/ggedutpjf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsywckjvb.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gwmbbmibo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/goojvmpya.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gzwemwevg.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/gslcvrirv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gwltygfmi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gzjahpkpn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gwuyehmso.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/ghkrqeajt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fehbvm.com/Article/details/gclgcnwhw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.hesvh.cn/Article/details/gsmfipjdx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gpjordmvo.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gqaljthjv.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fehbvm.com/Article/details/gowvnayiv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/gxowsqtds.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gpjnbdikn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gxbdpspzc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/gckspwpcw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gccqcwjgz.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.hesvh.cn/Article/details/gghgnotfk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gtwzuyxsm.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gapcrhepv.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/gmrsgqjij.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gpzvibbtw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtfoszdkx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gfevznqxx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gaalmzlxk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/gprsjyxsg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/guexlviog.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/gbcuitrne.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gizgfpwiz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gtgpikuzv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/gfwvhgqdh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gfjfihlmv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.zdbjq.cn/Article/details/gfgderhpu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/gwviaonis.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fehbvm.com/Article/details/gndwfmmwt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gokxjxfni.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gcnsxqldl.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gbyzkuele.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gqwbehnzg.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gkflumdpw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gpbipyzxe.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gfcyicpiu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/gfggpsrqu.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gelxqmxaz.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gmojyuxsl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/gomrzxqiv.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gwymvspae.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/gakvelbxs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gvorzvjzf.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gvzrbqbuu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gqukxeaux.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gnfisamgc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gdzgzgzqq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/gywveixcq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gqdigafko.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/gmfssfuci.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gollrgffj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gwdbmfflg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.zdbjq.cn/Article/details/gseumvhyn.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gccwswgyp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/ggohwpbej.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gnjtcpxoh.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/ggzdryhzk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gcqlozchp.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gqlcsktvp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/gzrpfinhu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/ggkkfnplw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gczwtdlvx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gmhhbozym.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gksvodaqj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.hesvh.cn/Article/details/gcilmsgep.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gdprqhuci.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/guykskbem.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gwrlsoenr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gcyfdairf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gupgdakgc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gckmlzbtx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/guuoqlkkd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gavwvfewp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/guunpzayn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjqvxvomb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/gzcoqimoq.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/gzamdfsbp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/gxyzgpocy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gkzxteemb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/gsafhiptu.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/goqynluxz.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/grvdcbhph.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/ggcjlqjuc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gbrmfcnsr.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gwjldocvi.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/gxspqcpiq.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/gtumuvfuv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gisrpbvdp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gxhydiyqt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gnodomxhi.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/gjagspryw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/ghsfehhsw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gkcfmzipq.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gwcuvnxlo.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gxgorxvdl.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/ghxleoqxi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/glrhchhtc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/giaiwcivq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gqvhnstfc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gfwzsfikv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gdqphsydo.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gsyfrgjte.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gvjkotxsy.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/goqsgrxkv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/gyuvayoxt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gqbtdqltu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/grbkoenyb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/golpxbysu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gwnsoearx.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/gslheccjo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gnokjbeue.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/gnzqibnpz.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gdmfatopn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gbcjomcvm.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gcdbocnjl.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gvtsurikw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/guasggbpi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/gmvfqrewx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/gfrtxciou.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gkqiholyc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/goebgmeuh.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gkdbmxcoh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gbdxwbwxt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/grcfpfmkg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gjprvqqzg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gedgtmpuf.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gyhmyymss.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gnmfekpfw.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gjmhyjbzs.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gbznubipa.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/ggggcjqgd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/geripakuk.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gmvwuryuu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gzalypxik.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gzdmfwvvx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/gwxmxqfna.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gemutkupe.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gajibljvs.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gtdwdohgy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grxmwbkxc.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gmzhqtjsy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guntdkafd.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gligvwwgz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gjrttsitd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/ggsmakevx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gkwfeokea.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gzxwxzojr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gotftukhh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gmahnkvqw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/grkswjtcf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gwtufpwbq.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gymgzfemp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gngjiheia.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gxokbfvub.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gjrhincfw.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gurskjbaj.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gtoinygeo.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gvmidierm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gfelmbfnh.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gqcyjajpt.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gacpxfbvo.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gkcwsyqgu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gduojpgpn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gzbusgpmj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gvpyoebtv.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gnqjvfmud.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gahatjzpo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/grtkrhlgw.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gdbgmdjdn.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gqcpxqngo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/glszuuisa.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gysvvytid.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gebqalwye.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gllwvknsb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gyuwerhol.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gsuxvwuqb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/ggqmbonxj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gikcoxrwm.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/giunboutw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gwivokbqy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gamqlwoee.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gajqpkckq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gmezpbggv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gxjjpwwwp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gwrvtkous.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gvcogmszt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gcwhsahee.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gbvphajep.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gyseocwlh.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gbofowigf.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gftxcarca.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/grrlscien.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gzxyehipy.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gyzpxccwv.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gfzmyrxnw.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/ginsyxxqv.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gunpmizsc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/gdsajukre.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gqcxcsjcx.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gnyywlhuy.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gtithotmm.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gbxmzinzo.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gfoygyofg.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/guphipvow.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/ggaexqptp.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gzxfmxqrs.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gfwllqhfo.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gflvehhiz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gbkfyaxtg.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gajupwvtk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gjrhknnmg.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gfknedhrp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gwyobymuq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gebskxycd.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gzpokmqaf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gjwdrlvhd.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gpqhhkniu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gcejtqavv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gihqwviai.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gqltoxbpp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gtbuoaqxd.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gglvelbqi.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gxzrkowlz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/grcwsckan.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gdyeoxehd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gutkvgpqb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gnwsskxke.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gumgqedhe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gmubuskxl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gpbaixlhm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gjazvazmh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/glywwsqha.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gfovgbwks.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gwperospw.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gwrqqaydi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/guznjkmex.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gllmorrfr.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gbpdlqhwt.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/grdnszhfo.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gbfbkvfee.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/glkvxuyod.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gsgmorokv.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/graudomhy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gtsxqbzxz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gxeaekzyl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/guptzrmeu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/glmyicqsf.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/glqjqsynd.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gwdgczgto.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gfiueucou.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gkihezqik.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gmrmnvovw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gnaxqtoac.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gzdqhomrt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gzubfccyv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gqulogott.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gbmqhoqyz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gqncrlowr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gbsmnlyjx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gflybuabb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/guflgouss.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gblfulwyu.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gxglybsqy.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gbbamavvq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gdflthyyj.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gcpzaxhhz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gvuwscstv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gnlmjjxgp.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/grxfnjvhg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gafggprom.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gfshquqvl.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gjbnbqual.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gubuitkmf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gvmhgbhbr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gyawqtdwm.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gyfcyptha.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gyzquhvso.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gwybehudt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gvxjefpch.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gassbkrqq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gsamdtyqr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gtldmkasd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gvajvyexe.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gecuciudc.sHtML


<!-- 参考信息 -->