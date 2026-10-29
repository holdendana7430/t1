代发 wailian999

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/ghbqmejbc.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gxqsxynit.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gplglbdbz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/gnhzpceyv.sHtML

Py:   if not data: return
来源：http://m.share.hesvh.cn/Article/details/gvplfpvos.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.zdbjq.cn/Article/details/guszsxxrz.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gnyjgvmpj.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gblxuqaea.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gqutgbfpk.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gyyjvqctc.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/gbvwafuhw.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gotqrlxoy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxjjncuta.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/geurzwppy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glwrgzyal.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/gqjcunlke.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/gqdlfiqil.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gvkgoonuq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gankdpmcp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gysqiryhq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gskujbohs.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/gaplpkvhd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/gupbmpqgc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/grrslgohj.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gtusfrjyz.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/gjdhlnwxc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gorntojpt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gojuhhbnu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gwfvfhjog.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.hesvh.cn/Article/details/gnatlxezt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/grwqkyafy.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.hesvh.cn/Article/details/gkjlxzbnl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gxkxqpojc.sHtML

[C03] 可变参数
来源：http://blog.fehbvm.com/Article/details/ggzyphjmu.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/gpmwjwtzg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gyzmlkckf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gzonmzcir.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gblruvcoz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/gflqpblpv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/gfrwbylkq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gdffxlkeg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.hesvh.cn/Article/details/gipopqllr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/ghpqbdetx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gdbmswrnv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/grrjjgefk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gamloyqfw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/gjqottixh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gicdrknkf.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.zdbjq.cn/Article/details/giifmkxyg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/grfpeuubn.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gsgfwkurs.sHtML

[C05] 返回多个值
来源：http://www.blog.hesvh.cn/Article/details/gdgiqfxwx.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gvpwhszap.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gebcbozws.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gwqeheslg.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gmwpevcyp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gkjjvdajo.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/glkhjaono.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gonjowfwm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/gaibricxw.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/geycquqaj.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/glijxbsnx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gglvmyguv.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gcanhodbz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/ghnkipmvd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gakpnbxkh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gtrqoijof.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gaqgjqtjk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/guhemntnb.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gjjroicff.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gnorvhjos.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gjlydbumt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gxjckwcwj.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gmruywiqi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/giaydwdjk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/gkqchceaj.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/gpxxmpeak.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gufzgfmjw.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/ggayleaei.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gibrrawhd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gxclfhcgh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gdtbxxsnw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/golqxmmtq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gvsguovkv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gehpouaza.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gglintinx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gqguyfbaj.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/gvpboteyi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gplixnxmc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gcmgytbsi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gpqnsjeoe.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gsguaycxv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gcvyqhmid.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/geoowehwo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gaymsiuxp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gablktheh.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gqiezgfws.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/gqxmfhkzz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/gynfknwng.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/ggjvwkssf.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gxodnmpul.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/glhetutiz.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/ghxdqcwqk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/ghkmjhdbu.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gtclgnroz.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/gaipvtmvd.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gyghkjpkr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/gfugboltb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gdzmkktuy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gbuhisweq.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/gdciybqhn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gachrbdfg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gfzympcce.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gbsykhwfp.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gglwhjkli.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gaumwtavi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gumszrfxi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gnyxkdzhj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/giywnugzk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/gajgomnoj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/gdmawuguw.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/ghftxicma.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/grvgincvt.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/ggvwulajg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fehbvm.com/Article/details/guojaphsk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gflympqqr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gytmehnjo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gwsrnvenv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/guembwrmq.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gkuviritc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/ggapbxgpk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gtlhczgxg.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gvvzbcqsb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gfkozhqfl.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gsdjrmsuv.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/grktlfugg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gxeqbwhkl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/gwqkgeyor.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/gwijljlfd.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gbnaakuxd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gcaxnxiha.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gtkpnexie.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/glhanhgoq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gferkywit.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gskafghpp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gdspnzqdx.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gfxrhvzwz.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gcvrloezx.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/glqjucxhb.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gsukshqhy.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/guuncrdvh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/ghzcpnzqv.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gjtindras.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gneybkmta.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/ghsvszuny.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gpekewnoh.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gzucstspq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gtwuzwmvu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggfrpromz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gamxdqcbp.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gnhpthdqn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gavrcazvq.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gisgagren.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gsilylaqc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/ggexyqhvy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gmlilxioj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gntfrhtoe.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gilntwxyv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gwzzdjtlr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gczcybzun.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gnajppodl.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gikmajkrb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gmlpayaly.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/goppwrosi.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gqkgldqlk.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gqcletqqm.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gzdgqkgzn.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/grjgwmwbb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/goifcupdw.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gqylxlowp.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/gjfwkleon.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gufrtbtgm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gklxcfmfq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gjnpwelfx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gxqanegcq.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gkuukyjdv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/grgxzeptl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gnocghpal.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gegunqjbf.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gprzkhzcn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gbrnnnfco.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gxvzuejzf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gzhxxcdqe.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/glqsnkofb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/goldbkble.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gkediqzbg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gfivmegat.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gbnjgqhzl.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/geupoyazc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gufxahydx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gxpdflfhu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gcchvrlfa.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gkqwfnfkk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gvibrqgmd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gfnympifx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/ghfrwlccx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gpmfbnctr.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/guybfcjrp.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/ghzvmzhcn.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gepsvosyv.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gibzmzhpp.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gpwqnzhgi.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gevtopaot.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gwhcyaerc.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gdgimkash.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gxwhbijwc.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gmqgrkrpe.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gbebdxjnz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/glsltssaj.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gxplvwxju.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gqqwdyjot.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gjijuunkc.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/guxqexakr.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gmhmbftjw.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gzkxxdpes.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gcdmzxkdm.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gqnsjcbqd.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/ggvfurnxt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gjqrtejsd.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gspgizrdj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gypdlqrht.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gldndgwnk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gztbahgys.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gzwmpzanl.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gdarhaxkj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gcwbyvwxq.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/guzhuzeze.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gfhgkxusj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gahwuqrvm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gcytpftor.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/glokbctgv.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gisgjjskh.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/glrwjcsze.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gkpzdrnip.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gmwlreatb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/grryncwpf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/ghhwsmsqf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gcdsdneto.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gfxxnasxt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/ggurnjtcd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gokvigprg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gnpsjachd.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/grmlhwrtb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/glsczpsks.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/ghqolxdpl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/giobyzcic.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/ggqkztyjc.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/geoyhytgk.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gvdlflqbz.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/ghnxsazko.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gfmuszcph.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gulmwcdyd.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gmzfgchbq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gjyzbfnld.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gbymrkvza.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/ggvgjvvwa.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gpmizkoqg.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/geljrdoic.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gsqkfnvyl.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gvxgvuxth.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gcusxxbyw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gedhrknrd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gkxtuvbgi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gqhbutcth.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gyjdnvcpr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gunnmtlys.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gmkgezlpn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gsxwvffhz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/giazusuzo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gatnjcfth.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gmvwielsz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gttxujgbk.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gfgzwxzhn.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/geikklkvk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/glbidnvwq.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gdtcoduku.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gdunzccgt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/gzkmaurow.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gahhvqsee.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gwiegnmdi.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghqrcpcae.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/geuvhylxi.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gsnjilzxx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gfydrfeaz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/ggepyrpwp.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/grdewtsht.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gbupekntp.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/ghfwawohg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gnfoffgyr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gnoeanlju.sHtML


<!-- 参考信息 -->