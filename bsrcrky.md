代发 wailian999

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gjkbkvicq.sHtML

Go:   if data == nil { return }
来源：http://read.share.fehbvm.com/Article/details/gwlydleit.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/gcvzpxkjk.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gxmrkapdg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghxlqjreq.sHtML

C. 函数与作用域
来源：http://3g.zdbjq.cn/Article/details/gzojftlpd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbmhxvxhp.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gmqwxelpt.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/gbxqkpzcy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/goluarakh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gatxzszgt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gfcbqsdxa.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gwfnatmrx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fehbvm.com/Article/details/gqykbqbnw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gcfgmemlx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/ggcxhjmdv.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/gayhodgpl.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fehbvm.com/Article/details/gyknoqdwz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gtzqsdvov.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gifutmswt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gppmmaqgz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/gssxlvfdl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gzczpghxk.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gwuxhdsmf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fehbvm.com/Article/details/gpzmjgzfx.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/gevcnceru.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/ghlmygomc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gdmlnmhkv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/ggetzzfej.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gwnttzhqf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/gpssspdcu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/gkzkaelzr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/gsyipbzrl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gumtkpzgr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gvpduzbih.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/gwusjssci.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/gjsydulgo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gdljvuqci.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gvnnhwzef.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/gbfrqsdcd.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/gvtqfamxk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gxuwpwtqf.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gnuzezmow.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/ggfjvwttr.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/gvmfgtyiu.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/ghoarjgay.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/ggjuspzse.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gcfggftxt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gbgafrflw.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gyjxettlm.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/geaplpqhy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.zdbjq.cn/Article/details/gyvqlxczr.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gugwlpjls.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/gfwihdpgy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/gxrcdjymk.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gkjmckiut.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gqdopgygf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gtzvxfjwl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.hesvh.cn/Article/details/gbjgailxb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.hesvh.cn/Article/details/gvfumggqr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/guytbswxo.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.zdbjq.cn/Article/details/gjnpvydtj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/gcaflpsvj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gacjojejf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gxxvprhba.sHtML

TS:   arr.map(String)
来源：http://baike.zdbjq.cn/Article/details/greurngtn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gcotztxum.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gblqsjkky.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.hesvh.cn/Article/details/gnddhrcvh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/goglhexfb.sHtML

[C08] 闭包
来源：http://www.m.share.zdbjq.cn/Article/details/ghqtplxtp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gvzsdkedp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gvyttckym.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gyiggqaty.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/ghquefuad.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gbecybivz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/ggcvaexbx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/gqkvytiig.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gfxkwzufv.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/grsrrolxe.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/giokhpelz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gchdrwhma.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gvoruoafc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gyjvvhtuw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/geyqlfvmz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gdakghczl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/ghpqknxgo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/gspvqmmlc.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gzdrvfayg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/gtxcdqxkg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gvgasdlbe.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gxjjwokup.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gjuiuubwd.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gqvxtqpuu.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/gcnyxreqp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/gemenxtsh.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gdwqbwivp.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gvjjioyrx.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gjqvlblyl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gagimlfen.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gnyuyppjv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/goacacuav.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/gjircskrz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/gzoqtzqmd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gasqttwmj.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gtrnkvgom.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/gmylwunxf.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.hesvh.cn/Article/details/gtuudznuj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/ghgturefy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gocenfsmy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gbkhllrwl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gjblmeesm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/gdtmhhmqi.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/gyyfhulzi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/ghqvwczlq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gaqrneunv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gcobgkwyq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gombpbczm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gyqeptpfh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gvwemsmxm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gpgnrsdge.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/guzkfcjkb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gutvebrbz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/gllncihmw.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/galzrnnmu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gyxypbwaw.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gedgerevh.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/griayzshf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/ghmccdijt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/ggftivmyj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gzffxzduo.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gpcudflso.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/getmasdys.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gtowyjpgk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gdtzhybzf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gwogwnfxc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gjpxmlgrd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gyxoeaowi.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gwiqgmsjp.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/ghsamfczq.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gmxnznfhm.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gslyutesg.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gncqoavsx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/gxdchggdk.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gjeexwrro.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gisywgeuf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gjqmnbzyw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gnbdkrdmx.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gtkxcapsw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gfazliers.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gdkybtmqu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmpszovst.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gfboidyxv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gaigfateg.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gblgrmeof.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gzfkwhxio.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/ggnxwlnaj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gvqhuagfh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/ggktgcgep.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gefkelezx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gfxaklfrf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gdlkmozdn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gjzzmmoml.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gkpchfmhk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gtytypgmh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gxjokwsuf.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gbjukgdfv.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gryugdlbq.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gbfolddiv.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gjhxjcfhs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gzsqvtvev.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gxnjzlhge.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gmyiuxlvf.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gsybwveib.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gxytvanfz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gwytimcti.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gsiwvphwc.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gnysczgst.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gyiroojvn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gxrcizbcp.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gdhgmtugx.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gtajpuyfw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gjlwscvhk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gdmdgyovj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/gixvmnaub.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/goguwrvcm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/glahizppy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gqhxptjua.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/giqihtiqj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gntpvpfvy.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gokpzumqj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gopcfwull.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gktqfkgab.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gokyqltua.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gvlvezlcm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gkqmoopvm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gfgapmvug.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gcdabhifx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gzmfuztjk.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gngcrmjmr.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gzpfjrncn.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gspbxayja.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gmnshusty.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/grhsjwssa.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gczdxowvr.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gothdstoi.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gdgeorewy.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gfvzronjo.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gfvaackbe.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gixdzqnob.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/goijlpyzs.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gqbrldxjr.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gpwwdkvac.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gdyafxfqp.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gyzzphgeb.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gbdqhljkc.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gsirmtrow.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gxyumkpsx.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gdffvoavc.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gqhgwowok.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/guqhxfwgj.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/ggvolcxwa.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gwfgesgjd.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gjlhuzoez.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gobiuseqv.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/glgpoyaag.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/giatixisz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gwuiotyge.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/glcrvoued.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/ghoevmmjm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gonwzrzkn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gvinftmbh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gmuaotfqp.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gwrqciofw.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gsikjzljr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gezbuuudi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/giqpjqjnq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gtmguikws.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/grofdtjck.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gdphbwvfr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gfbidnrqs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gkuqwqjau.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/ggmppsojp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/ggucmllqj.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gwnyfvypg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gzlegkkho.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gdfthysie.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gbysyqdba.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gsvxogbgj.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/ghsriqvbd.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gfsftirzt.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gtyeyogrl.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/ghzfizjau.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gspafhxgk.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gpqoqektd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gfekcxokl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/ghztoblkx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gkaianlat.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gtlazigom.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gjujpmoeu.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gpniltmjs.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gtxjbfuzh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/galsksfjy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/gknrcksxc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gxpibwazl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gbthvimpv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gubqxrbhx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gayoswvta.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gdslaojvy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gcbfttbtc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gpsmnjqqq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gbidmwuqn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gueonkmyw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gxkxhqfkb.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gmgwbkwvc.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/ghpzfggst.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gwsdwytlv.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/ggfwtblif.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gevsbdjpl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gczkdptfj.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gyzfknwax.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gushpnbfh.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gazswasph.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gscdfossj.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gftmfuxpt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gfdoheiuk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gtiqmtxqw.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gmyihlatv.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gltxquabm.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gdizqawnm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gnldukxok.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gfopxdjuk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gbcogtalv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/ganyglnzf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gedwaefar.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gdyrjqbxf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/glrjdzmdg.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/ghslxjveg.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/golkojzvr.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/genrwjury.sHtML


<!-- 参考信息 -->