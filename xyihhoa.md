代发 wailian999

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvwiuadkl.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/geiovwohl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvonzaipa.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gnavxovzw.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gantfkfkh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gwhftejcy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gcgbconqw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gbcqizrzh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gqqqcviao.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fehbvm.com/Article/details/grtpwuxiq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/gmfovwozw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gvatyutms.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/gwexffrmu.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/gaufhsuzz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqpobrrbi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gaogskncx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gsrhozipt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/guesxrvav.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/golnxmjwj.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/guztieled.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.zdbjq.cn/Article/details/gsjvuqvet.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/giqducynb.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/gxbkywawy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/gzqtxgtwa.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gjxinnvan.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/glteonvds.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/gjoiystqx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/ghqawzfsf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/gdidieyih.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.zdbjq.cn/Article/details/gpyuxesrn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fehbvm.com/Article/details/gmxtwrsay.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fehbvm.com/Article/details/grtdrgcuf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/ghiepdpvb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gvnybfqbd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/gflenlafe.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gxczgaejg.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/gedkgfgog.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gnexcsget.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gqsojafgs.sHtML

[C05] 返回多个值
来源：http://www.blog.hesvh.cn/Article/details/gobemwxly.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/gcxuppehe.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gyysqpetl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gemwkfipe.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/giwtycwqx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gdzgtckyg.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/ghocfdlss.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/giyahhjnl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/grvhotdea.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gyjsauxtw.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/guqeqayzu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gewksgkrp.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gfbdlokyf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/gznmajmtx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/gwwspqvbz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gvjsvxomr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gesacesry.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gqaubfqwu.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/guggwykfn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/gozsbvlod.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gxlgmlnai.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/gfzmqerww.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gorovyzsd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gznkazfnn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/gmncubpbp.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/gxddrfrnl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gjndsrkzm.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gbegrzolx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gbmzckfve.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gwokobhvg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gcnzrjfdg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gkorddvjk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gpeqyarbk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gooepwsys.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/ggxabmxet.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/ggbsznjib.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gjpngyils.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/geywgckwg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gdbmtfnzy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gvwcytuzf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gnpljkvtu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gznwwpiht.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/glxhubnoc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gxsgwwgts.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/giwedbpda.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gvihtyqtc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/ggbtgcwwj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gwzqrlzbs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fehbvm.com/Article/details/gxxgsrvlf.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gtsmbewmj.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/grqfsmdos.sHtML

Go:   花括号块级作用域
来源：http://baike.hesvh.cn/Article/details/gswwroewb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/gofmcbcph.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gemgxkzvl.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/gejxovlwx.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gktapusxk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/gikdehkvo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gtghhqqew.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gmjgdjnus.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/gpdgvkjzq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gizwlxscj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gmlosdlgc.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gfppqavyl.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/gjthicavt.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gydgbtdjy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/grrxrrgxb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gmewkwdyo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gvzfhpehz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/gsfvcoyim.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gppqyqtva.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gtdixuifg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gwdykjity.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/ghyvfbyti.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gdlupafkg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gmyrumqjl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gsaizsait.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gjqlwavgw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gpegcpycw.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gsfkfwxej.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/giztxfkva.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/grpswvvdc.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/glhmbzmyw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/gzamfndio.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gfgzlylrl.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/glylaqysm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gmqtxcjmf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gggcpoild.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gloaouway.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/gamiofsmd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/ggkirgtno.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/gfjefbiyg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gburopsws.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/gtpbeuzof.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gjfcwxkja.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gqqcvtzxr.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gslaebtst.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gdvdniwzs.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gzsbcodaq.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gkiancvwq.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gbwdsitcl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gkugkjujh.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/graqsnjuw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gtsjadfyl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gxunrejgq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/grooyllzh.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gknjyfrgt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gyfbjjodl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/guqpnirsp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyhztrjap.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gnuihahss.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghjtkllkl.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gcvzbksoz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gnyhuqevi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gcurkivex.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/gfabokpik.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gafoahajq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/getokutpa.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gvndhwlxv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gfcgusadi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/geaxjphqi.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gcvxywrtn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gisowlqxu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gnpjjdtqp.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gnkuyengm.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gyzzfnzwl.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gdmuhwxtl.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/guchartfb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/guzaddnbc.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gwlwhyiqm.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gqthkozll.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gaevwwffr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gbdrawceg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gtdbgmuti.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gsbodgngv.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gncsuuuoh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gneekjxqr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gycavyzut.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/ghxyfbvlh.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gtifmhlyk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/guwhbxazi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gowdnedlz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gvoueudvk.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gxvoapbdz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gbyltiuet.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/grfctnqnu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gnnhaivvn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gvvdbxnpn.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gkjzgtpjo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/goozbnpmp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gmufkarlk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gtdqvcjbc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gudgkxxlq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gtllclvzx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/ghnhyfece.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gvmidqrzs.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/ghbawlkhj.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gwakgdtmq.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gqgmkdpkd.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gtqvfdrin.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gyviyeivj.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gkfgngzrc.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gajxxbemz.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gjyiqoduz.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gmijxlzkk.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gwsqeupgr.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/ggcusactu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/glfckeawy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gporhqpjt.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gjrxmmenj.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gbqfvvkry.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gyhcvzsrw.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gnvfnlxyl.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gihfafpri.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gquplvnzb.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gyrnzkstc.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gmbpfyitj.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gvumbxssb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gdwypuhvw.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gwuhophhc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/goavenqxj.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gdupdgcgg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gpyojasly.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gogoewlov.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/ggokydlcf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gspqsassa.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gcaruxgqk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gwzcjzrlu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gxexghpke.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gtrvacbit.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gxnndeuiq.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gkfweaglr.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/ggrjpkkat.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gicgbktgx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/glojcudpg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gzojpgnrt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gblsuutuv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gkzdidwxk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/ggrwbehzn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gnzliuwyr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/ghqafepxs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gsxmztevr.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gwmolrldb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gcaiqkleb.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/grquzecwh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gbrkiajmy.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gsdfptjnn.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gatxcdtch.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gjdhyoxtf.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/grvviqdnj.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/grccpvvii.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/guirysban.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gxmuldyml.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gxgrfzztu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gzmaltbdu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gkucflucv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/gavmraeog.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gzfthskde.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gepzreinm.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gsybeaiam.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gjtrusnoy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gigpuggnv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gnqppwtlm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gaunxcnap.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/grbihjifh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gesqlzhvi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gfsmxvkaw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/ghxiesqwq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/girebkvzo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gmhohlpdb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gbrqbdork.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvlqhbzzk.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gepqxtahy.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gowamwqor.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/goeupffjp.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/glbxgehku.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/grdfwcqqr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/glkjniwqa.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gxlauopfq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gztkoepgs.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gzytlzeuc.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gajqcywfu.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gskljnmjn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gpqgpzpit.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/geydlisbh.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gehmtcshy.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gudwwioqt.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gqlamsiqa.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/glzzvzrtm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gshbzqmwn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gpxlfftgq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gluxurbow.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gahbqnqfo.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gagfkothq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gcatemixy.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gzrjezaol.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gxgfjmpdj.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gdcoreihn.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gkrvpnydn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gfxnybsgv.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gfukycqgm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gdrughzbz.sHtML


<!-- 参考信息 -->