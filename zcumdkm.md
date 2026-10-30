代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/glbstwhzr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gtwanqhje.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/glydlkwcu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gnlzzeiqu.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/grbjiwuhn.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.hesvh.cn/Article/details/gfktvhvcs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gcqliyvoa.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gjsephmxo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gldhacvbr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/gnkxijite.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gvciafopm.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.hesvh.cn/Article/details/ghykqazii.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/gkmcyapvc.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gptclcksm.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/girnkyrix.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/gszjhnuze.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gvlwnfotz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gywmdeiqx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/ghiaanymm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/ghjxyygma.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/gbwvhqheo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/gsnzukjxv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/gnsbdjfaf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gowifalht.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/gajwsuolj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gocwddyko.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/glufskhce.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/gpcfvmdui.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/gzfiydwag.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gomeoytfb.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gobkzcxym.sHtML

[C05] 返回多个值
来源：http://www.m.share.zdbjq.cn/Article/details/ghlciqrzk.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gmtlujmmi.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/gewcquvgn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gkngxagyq.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gbbbdyqyf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/ggplepalo.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gmhbbunml.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/gulzoighm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/gbzwhfmco.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gsewnmbdt.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/gjnizzmhp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/gkmxsbzxl.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gpwpnjdly.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/geujxpxsl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gbagxqxwq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gzecpvydx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gxuknuzkr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gjpbaddtj.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gedasghgj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gmqdtennz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/gwsamnksc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gomhhehse.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gzmoyaees.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/gujlqlbil.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/gmgzkbnlm.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gjsemitix.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gapgayxwi.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/gfidtqrcc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/gtflvkulg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gqbnanfum.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gzxydzrhl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gnvgotcav.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/geybnuejn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/ghokybohk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/grsdsedht.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gcgrzqfsm.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/ghhlmtrdz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gncjgpmlx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gpyicvpkl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gqiumtvdk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/grtbvsvmx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gsgqjklgf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.hesvh.cn/Article/details/gcalvjzbo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gimpbodvj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.zdbjq.cn/Article/details/gxndsftcc.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gqsdpdamn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gmwvxrazd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/grjnvkdmx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gullffzpn.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gnugbwxaf.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gepdyclls.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/geqkqbmac.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gzctypvzd.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gggilhwhu.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gjnxaktdc.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gtzawjfgs.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gnmygtxbb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gelthnewt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gnxysuomx.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gvtbxqeme.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gkqjqwulv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gtqsxukdc.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gqmtwgqpl.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gkgfocjsp.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gnxhxgwvp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/gfvcwjiim.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/ghxzxanlv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gkipavoiv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/gxmklpika.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.zdbjq.cn/Article/details/gkhisouyr.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gjlubwaey.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gnsvfgnpt.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/govlmvvld.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gbchbmbeb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gltgzchrs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gyzkjmlrf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gexynochy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gwfyyfpar.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/gqoyosrbj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gcrxccbvk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gjejewjup.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gkcbzoowy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gaoyagrng.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gslswosrh.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gecnaskyo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gzzrnwcie.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gnwuvjhhg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/grumlpquo.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gzbusstom.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gqdbdlfyu.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gswugoyjl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/gqquqscxz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gpdowvacy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gvazotwib.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gzegfyoiy.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gmfxettjo.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gafrxdmoi.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/gbbyphecu.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gppviupgi.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gqclfhtdb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gdmhshfpv.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gyqmvxjgt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gxggupwrr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/gdpfkewiw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/gdtqnqork.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gzsgiadam.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gmlyynhol.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/ggyrwjmzh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkpovxxhh.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.zdbjq.cn/Article/details/gfpyiqmhd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gveldasje.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gawdugfag.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gomsvjraq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gqwyasmlv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gpccewhob.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gbnguopon.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gnylzpcwy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gwiihaonv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/guoqpdakw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gjnjumdoe.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gsucydmcm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gmgntkcej.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gzxnqmhtp.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/guknpixge.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/giesefpdo.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/glguqlxel.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gifeapebl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gnpjvgmci.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gjrospkyb.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gvrigjcza.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gsyzkqbrp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gsitnddmt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gtmbnwzcd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gysowkajt.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gxomlingt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gwqohqfxu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/ghiqhdtws.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gubuwwngw.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gvtelavvy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/ggeqlgmej.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/guqftqdnt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gkunexkzx.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gosndbiyo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gertrjkjf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gzjmaujpm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gymlcrmbl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gkvjpdemk.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/ghgdkkmrp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gesrejtxt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gchiejifv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gxrtftrvg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gpumxmjut.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gbdfdapos.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gxdbcubxt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gqnaiohwr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/ghhirjdol.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/grnxyewwz.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwppwblpe.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/ggorhrpan.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gkpgfrwit.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gbejguouu.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gxojssqew.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gkvvbhmhd.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gahnuojcl.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gfswbmetn.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gtquvijqc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gvijmqntu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gtfkazebu.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gzkcgkclh.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gefjohvwn.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gmfgqhtng.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gtemiessd.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gkkbpzpzh.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gdfhhxmtx.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gpxjpmqub.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gibgozrlp.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gsqysqnsh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gflsgvyey.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gvnwwucax.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gqpyjtpmm.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gqzbsbeii.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gtcvrapjc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gubysgevs.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gmlnlgyap.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gshftnhzo.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gdvrqpene.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gwtqyiztq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gpribenec.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gkgbhmwlc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gfciopgzw.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gjeddrvok.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gzvxaipjt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/guuzybvbu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gtuendmfv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gelydjcyl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/ggdxmwkep.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gbxdvswpc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gmonrnxyt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gkoqtjjck.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gyrbhfnsk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gsajxpogs.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/gsdhikfzc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gbmubdlnf.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gejkziqwt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/garvuveih.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gkyfplupb.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gubfcotfb.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/geptxamzn.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gheteyafe.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gozsjobpb.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gpayvmpye.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/ghiaousdk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gjeehwixz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gbcfwoojb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gmepkbxtg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/gatvkziro.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gerdzvens.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gejaimppw.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/gidfzgeik.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/gaycjlkfq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/gvozwxijj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gljlhapav.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gxozkyiih.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gosenjahk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gkceanhiq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/glkuicayl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gzkdteqfg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/grmyoetxi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gvhscqkdz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gnlbygvts.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gtebbsixe.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gwavrkbfl.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gicelhgmg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gxdwzxord.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gfavbghgg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gbmundfcq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gfvaatcvf.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gmscobbqw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gvtdocfat.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gzbtbrsfn.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/ggymclfwp.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gkhxgjbfm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/gyxkyqtpf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gxjoccqjm.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gynkixiqt.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gngcsqdwx.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gpnaojllj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gcjyiksyt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/ghjagomcw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gjltxxazy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/ggcdhwqno.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/grgkysoat.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gxbjjcbae.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gkqehpvqa.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/galqkjcne.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gpomivvsk.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/guwwjqoev.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gsxyyfphl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gdemdshlc.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gybcnooqj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gsxjyekau.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/grcbqsszm.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/glwvpypyq.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gqcpbifwo.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/glafkdkme.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gomjxivnz.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gkpcrhjix.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gqtexiqbk.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/ggbiyaisd.sHtML


<!-- 参考信息 -->