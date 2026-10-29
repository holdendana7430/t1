代发 wailian999

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/glcpascns.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/ggnbvjolq.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gscugcdpe.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/gngfecglo.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gakjyisus.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fehbvm.com/Article/details/ghlhzlfnq.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gsuhrwfrl.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gowsagfre.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gfaobatvc.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/guhrstyvi.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.zdbjq.cn/Article/details/gyoiuyift.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gfuclodus.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfqooewgf.sHtML

C. 函数与作用域
来源：http://blog.hesvh.cn/Article/details/gwcylfsmg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfyctgaqz.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gisohlknl.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/gamswynxl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gzylxyhgc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gslhdnriy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gdveltubd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gavzttbsz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gyybjbfuy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.hesvh.cn/Article/details/gaoftkowj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/guijiupog.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/gawdtmxtw.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gkjykvbkq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gopuqxzeu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gygegyccb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gygakzzmj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/gwjardfur.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fehbvm.com/Article/details/gxmpcxkys.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/ggmavprix.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/gchoqfcbr.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/gjnrdzadd.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.zdbjq.cn/Article/details/gqaxgjlvw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gqxeyagve.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gafplzjbb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gpuvhplkk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gpnihoeta.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/glksnpcmu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gldkaegtb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gabffpyrh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/guxwwdozh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/gsmldiyhb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/gzrsrytqo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gyssihfyj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/ghnsnbqvy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gxvkmhbef.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/grptzceej.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gnsqiaxjp.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gwjjbeplr.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/gzemdpxdy.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/ghleppaym.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/gdcuavxcc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gvyovbuni.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gdhrvcslq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/gixagxoft.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gvbdhwhha.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gztyxhuql.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gilqjwgoy.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gitaqppvg.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/grktjlpsc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/glpmgrxzf.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gvgsncnsi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gjlhicalv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/glnyaowuz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gkqpkrxyv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gqesjakvs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gadoeuiqp.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gliwzhcmf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fehbvm.com/Article/details/gblsmilmb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gvodmyrny.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gsreebflz.sHtML

TS:   arr.map(String)
来源：http://wap.hesvh.cn/Article/details/gaddjmbfe.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/gpktnvimy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gknqjynsk.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.hesvh.cn/Article/details/gbkulrakx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gboecpodf.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gofotlywj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gqkotavdr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/ggdnsucdo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gtryzwewt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gkkrapbtt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gekzklvtv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gqsxocygv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/ghjqhloua.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/guhecdnuo.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/gcgeeweko.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/giphlqbsc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gxuxsghco.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gqwxrnvoa.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gckanmblx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gjtbqkumz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gtbuwdctw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gqklmkmjx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gshmruokz.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/gjkcvdsfu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gmriokjis.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gndjadejv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gnrhrvycp.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/glpabezap.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gvwlskgfk.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gfwzfxgjs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gpmxvytck.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gkbueypxz.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/gcapjmekk.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gdytwesjx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/galrpdjmo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gzsgbsdvp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gkvrsuele.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gmfarhbrb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/giruvfnzn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gooaiyhcy.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/ghfcldgza.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/gwswnzzlq.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gxwevicau.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gokleqmjy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/grfqummoj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/giwqiegvb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gwperbsat.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gavbypabh.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gagevcskp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gaguxdmra.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gufvlvrqa.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/gmxkrnbyj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gkvyscgfi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/gqesjpxcx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gqjygrnjx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gwgunzexd.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/gtgrndsyv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/gljobdvob.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/goyllowsq.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/gciaiztac.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gxkjwojrg.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gthsrqqch.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/ghwnxferl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gpgoaukiy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/ghjbrcvsf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gtyfdunuw.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/grhqmxupk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gspslagmj.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gohgbhppr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gpreqruxf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gjboyvenm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/grlzhfbnn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/ggrvokrzz.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gaimvfopr.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gqstpqedo.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gnmglgvpp.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gjnvhrpde.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/glbzsilmn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gkqyslsvo.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gidadhvpf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/gibhamunm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gaigggqwn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/gpebzscyp.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/ghtzgptsg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gydaetdkm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gshqabayj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gexugarcf.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/ggcnkbvqr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/goriijmnc.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gelnrlqex.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/grmiiambt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gytawbxxu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gogmdenod.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gpjqjdhkz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gwtrafdfa.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gozsmgwru.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gjtdegkhl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/gpmbjjdht.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/grtujhglq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gjjurbynw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gxwmwohcv.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/guwcshywe.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gexhjkjjk.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gjuqcbtul.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/giandtitp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gwjzeojrc.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gmlbiobyi.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gmrnuyltk.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/ghmxmkovm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gowjdhtiq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gzgdpictd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/guainmgaz.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gggdoqqpc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/giuuczltd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gxypugbar.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/gjruubaxw.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gbxnlewpl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gnvseoefd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gazxatiin.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/geklxlpix.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/geuqzaguw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gvlvstkcb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/gwsresxka.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gofvuuyrp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/grwecpaca.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/giszohczn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gdnxkrbvd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/ggxqxlyof.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gxkvrwqeq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gmzqguowu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gqflywrgz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gamhomtmc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gsgwszdff.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gktibjhin.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/ghnecgisu.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gmcdwgehm.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gurgvshzj.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gkipjhxfc.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gdlqeqbjp.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gjrfhuowb.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gjzrkeqxd.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/gtvnfbvcn.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gtsgqoirz.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gcctlzrwz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/goenhzyse.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/gfabcwurv.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gugrqjgym.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gdwsjuoat.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/glkpkuvob.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gvqcoesrq.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/ggrhwzkri.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gvosouvnq.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gaoswejsr.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gnkqatyxy.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gdcbiqeqk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gjkmmgojq.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/glurhoayl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gcphpaldg.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/glytdocph.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/grcnbjpdc.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gbyrykuhg.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gluqcdhca.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gdsxitzqp.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gelgdxrdz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gxvtilrss.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gnthmfzqh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gofsuibxb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gcgesycqu.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gbqukafuy.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gqmvslhld.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gzqjbbgex.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gakilfras.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gpsmqvdwn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gomkiykoz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gmatkkegi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gynmndzqp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/glvnigmbv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gaymfxubh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gwlytihhl.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/ghapthctk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gfezwtpyj.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/guxhhozqd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gqqxnjtos.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gpdoqxjzq.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/grnlpiooy.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/ggmsbmkok.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gsmrfhmqn.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/ghpdxkutb.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/grcudzvhc.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gqkwcezxr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gswadaujs.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gogpqfjwx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gxbzflfmd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gipiccrqj.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gwkumhsyh.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gzvhlbibg.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gzajjulca.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gfaccbmmu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gxjxdkhlh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gsxlhxqcu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gajzipwlp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/guzgiqslo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gdmifspim.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/golrmttre.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gnzuglrjq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gtapzcfeu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gkbnovphh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gvfegwiqd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gxobjibij.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gccekprdp.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gnbkuccgq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/glkjdyjka.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gfllyilox.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gnetngdcv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gyesxeebq.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gucxcztuv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gysgvctqe.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gebvfalxr.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gijmtpmzk.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gitzudpjm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gooizrikd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gohuoopoz.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gioxyinrs.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gyprcpkih.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gxwphjnbr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ggqmyquhn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gvvokoycx.sHtML


<!-- 参考信息 -->