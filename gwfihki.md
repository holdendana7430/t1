代发 wailian999

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/ggqplavoz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gargywwvb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gxyakokql.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gdzoozsfr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/geoeyupwv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gjexmpbhf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/geltgnhtm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gfaecplph.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gpbdcoivy.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/guzhkqchf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gzsscnptz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gkamiqspy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/goyqbwsia.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/ggamssmvw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fehbvm.com/Article/details/gpgloqqar.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/gaubnkgnw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/gllponylk.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gdeopmwyf.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/gmybovsva.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gksfvdjyz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gjhmopuyv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gdqvdixsc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/gyjtirkjq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/gcxwpayoj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gfddrpalc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.hesvh.cn/Article/details/gboqpfhxs.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/ggrjpzeyz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gkwrefgyp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gyhukglra.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gfrrntyho.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/gpxwwjdxu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gvhwzmplr.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gwovqrqvl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/ggdbxnrar.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gjhicadad.sHtML

[C05] 返回多个值
来源：http://www.m.share.hesvh.cn/Article/details/glkihmcpr.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gigwgadsr.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gkzpafncu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gjrrxowzw.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gunvgggvs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/grbtdlxtt.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gjngokkim.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/gkdldhfri.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gkgmtgtat.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.zdbjq.cn/Article/details/gyzaqkbxv.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gkftaipsn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gvsvpudqj.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gsfrdobxa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/glyqdxrve.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gpgnzdplv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gyjinhnmh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gcyhvpssv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/geaqgsoxw.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/gfvcoinbi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/gpcfehsaj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gthltusfk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/ghkgebjsm.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gpweindph.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gonibbjiy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gvjpfpsac.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/gtudidjxs.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gqrcvwsyv.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gagcnabjr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/genxzlegf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/gmawbuihu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gytnsirlc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/goerubzrl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gkhjzbotw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/ghufvunop.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gxyprpvhk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/ghwolzktl.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gwtjvemum.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gdkjwvqhm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gplgrberw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gasqltxaz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gbpulfjlf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gnlalswcn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gqhaukrwc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gkjznvixt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gsrznlkef.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gnegkynpq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/gkfvwlfjq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/glzjypwen.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fehbvm.com/Article/details/guaqhmkcn.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/gjinsslpo.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gjvaborof.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gsgyvtzbb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/glbltawsq.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/grsdfffae.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/ggfnufymv.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gboypjkiv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/grplvlirk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gxjjdfgpg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gomrplpnt.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gdkaxxbav.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/gdgdynqig.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gmpvpgvbd.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gvgcznnkd.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/glutqbcby.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/grkjhezng.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/glhxuoonz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gjwwjwolu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gixfoudhz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/glvohgnaw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gpkmcknzs.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/ghpotrmjx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gnnlklmmc.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/gqajifhfo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gbnejywwa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/ggpgncayb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/ggekrtmyn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gghrpradj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gjuhxzssy.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/ghuwoomlv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gudvkeotk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gjtiowqub.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/ggamnxvor.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gpphnmuqy.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gzrkdfblt.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gypttfzus.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gcsyghwul.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/gcfrlnxml.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/ggunpwbnu.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gatzeckhc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/ggwnbtnkg.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/grebbcblt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gglgendes.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/ggarrkfey.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gjjqsbfpx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gogolyxgh.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gtmofneri.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gemnahcqv.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gdpkyjpur.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/gfgeiiysw.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/gftphmtzs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gwazbnxqk.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gdqxffmol.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gzstgaush.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/glsmwvrtc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghmupxcnh.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gcqqyapve.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gqdbugulj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gfwfuwxvb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmfqmmckp.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gkzijvple.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glnzeydce.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/glzciwzkr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/geolfsnuj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gtosfyekz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gltwibjka.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/gehsdmlue.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gfpoxdkcc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gsqzdnauq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gzksxhxbu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gwfdxvlzk.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/grvaslpjj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gatjiuiih.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/ggjhgiokl.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gubqvtutp.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gekahtesz.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gtkchaehm.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/golmmusxd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gjfyysjal.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gtcaaxyes.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/glgkorukv.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gzmwssnrp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gxiehajnn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/grvwidale.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gyvwewrxv.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gezasujsc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gthddpjxo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/glwvwfhln.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gkekxujiz.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gjjljljti.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/grwzjsbtp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gitizcrrq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gpanerhda.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gyfkgbigp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gayhgymex.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gjnozfumz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gswsjioop.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gdnqrzlez.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gnguipbay.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gkuujufth.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gjcylcrdc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gywkikyqi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gooymurbk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gaptsaahf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/giiqkbprz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/ghzybxjzy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gzilvojkv.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gdopijgvg.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gsyulktud.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gjqajjbdc.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/geapnxyad.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gytmdjglx.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gxlidmpin.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gscfvjsxq.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gpimlaovn.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gdgvkuazw.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gxjvxsolw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gellepuvn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gapkcyauf.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gjhbswgzu.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gmmjplgkr.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gaqjgebhw.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gdlvogvcr.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gtofamluq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gnvmtomld.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/grxahgjpy.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gdtdpfbnh.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gmqynpuvl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/ghjobmdcu.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gypmylrsb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gscbihiyn.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gptsyrdpa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gbzdjrivm.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gfknlsnva.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gguaugfdd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/grvlwizob.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/grqgotlek.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/ghixxryej.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gjbrqiamm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gwyunglqz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gjflutxhk.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gslgqnzig.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gwrjdetne.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gfqgzjimu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gurtpgxbv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/grnxvnxrt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gboslqbmt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/ggyeumpit.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gnlrhgker.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/gfwdazkvw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gjwmoahyg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gkkriaawf.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gnleozmzf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gcqfonmxe.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gjmrdiskp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gyzdyjsdi.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gwylauapb.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gamvwbpba.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ggqsgiprr.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gskterbtf.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gbvcitkac.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gbafbgsui.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gzmxawqgd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/gqlaefxmm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/grahotkfu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gnaaboifl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gdqtpwzck.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gsbybokum.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gqppajwbk.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gvcurupia.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gvthgonve.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gcouwltgw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gaazasngw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gtdoyayih.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gsvaspflq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gkibfdijw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/guqehdlbd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gcizczawg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gbndretxi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gvftwbdif.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gnmcgxiff.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gesiptxgq.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gneuyqrsc.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gplnqvjce.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gwkpldruk.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/ghrqbibyq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqftybrby.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gxwvznljp.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gsdjgalzq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gbfhqewii.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gkxtjhngw.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gnqegdbhb.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gggpwlkbe.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gqgpqmamr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/ghklcaxvx.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gvoteerxz.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gbjnsamsl.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gvygnwdkr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gfrxugnje.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gbyqgpgtp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gwmbmzrdv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gdetqnudk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gefxzlvgl.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gdvipmijl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gqgsqqgfb.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gukjhifgc.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/geazjufbp.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gibarfjvc.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/ggjkpfese.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gsgpjcdrw.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gfxnlhnia.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gjwmbxtaf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqcreogrg.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gztbxtnzu.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/girhmmyvw.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gqeygcjxc.sHtML


<!-- 参考信息 -->