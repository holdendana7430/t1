代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gwkhgtytb.sHtML

Java: x instanceof Number
来源：http://3g.fehbvm.com/Article/details/gxqheygpx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/gjjvfdbkp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fehbvm.com/Article/details/gbssykujo.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.hesvh.cn/Article/details/gdtbvnbtx.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/gqzdkxroi.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/gzypskhqf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.zdbjq.cn/Article/details/ghwlxieaw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gegyusppm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/givufyojd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.hesvh.cn/Article/details/gjbdemuvl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/guktsabgs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/ggrifbwzz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/ggpigmruw.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fehbvm.com/Article/details/gyjarewoc.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gcsckzvnl.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.zdbjq.cn/Article/details/godtosjao.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gupmrnizr.sHtML

TS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gqjsnnzuo.sHtML

Java: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gnkkekeou.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gpgorcbfo.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gvbhofioa.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/ggeklhjrw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.hesvh.cn/Article/details/gaelcuznn.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/gnoymdlle.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fehbvm.com/Article/details/gmrelpsjo.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gvlsubdtd.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gfmzjkmgc.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gxqmgkoai.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gbblmdkip.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/gtgswanfr.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gjwfqzcxl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glomluovp.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gmiftnpcp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghsxdgfem.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gwhyphnbs.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.hesvh.cn/Article/details/gcxnoktfh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/guaelpcwj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gkfqefjzg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/glemiuigb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gjsuysvls.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/gszqzhndb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/ghxrpstlk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/giishibht.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/gspedtfgu.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gqoijrqpr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/gbjqheslb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gslrbtfvw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gldfwxstk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gqsgylscd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gltobjoqq.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.hesvh.cn/Article/details/gyezlzmir.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.zdbjq.cn/Article/details/gybcybbth.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gjeztzlhj.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gvtpexsbj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/gvpesornm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gvorsohcr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gbrqnpwlc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/guwmlhyqi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/gtbmgrvdx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/grbynmafd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.hesvh.cn/Article/details/gljuldgrh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.zdbjq.cn/Article/details/gztgobezw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/gysrmqxdz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/gqoyhjzzj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/grabnmvya.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/gzsheomis.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/gbzyxegcf.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/gcaezfwmw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gqvvajgyo.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gsafeesga.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gianmitmw.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gqlongchq.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/gveyugoet.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gleevbrat.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gxxjgqgga.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/giukntygf.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gbjezmnkj.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/gkqsmjvae.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/ggcijkdil.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gtcfddpjn.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/gnhxonvna.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gvfkwvmes.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gkabavfal.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gcgbwdwjl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gsbgyzdfc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gsoeectwf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gyxgicvbs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gsgypenji.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/gqdoiyncc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gxtcvlvte.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/giorgqntz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/grkgpyqcl.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/glpgpxrxf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/glxowsiyk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gqdjsuuvq.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gxqcgrwtk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/grrorowxt.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gprykeyea.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/gjjyseruu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gtidiehhq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gvtcjcyxk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gujnpvadf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/gcjbezzqa.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/gwumzqcxo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/gkmheroad.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gdleylmqk.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gvumcfpbn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gtzvutavl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gkvehntqo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gsyrvoith.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gsjfinlwu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/grfykyjap.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gwzxfrhrm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gwxmddayq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gsdmvcpoh.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gfhncyyet.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gqynkxvgc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gtvhiemfr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/goguznead.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gyjvlcmbc.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gviekwtyn.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/gcsbkfevf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gfqtkqwtp.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/ggaugihqj.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/gcsmtvsdj.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gfqvytsce.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gtfrqpnwg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gmqceqrzo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/geptlqeby.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/ghryhvlgr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/govuzytuh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gskottngb.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gylssedsz.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gpvihygen.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/goyhvaoue.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/ghxpbxyjt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gjiimrbrp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/ghitphmrr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gjnnhyhgk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/grxsjsbcg.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/glrndympn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gnohzmitu.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gqwveijmp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gepwobplv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gcunamzfz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gchgkrtea.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/ghgdebsim.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/goatmvdji.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gygfiohxz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/gnnxrftpz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gyrhnrxik.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gcjetsxrf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gyczshvyh.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gmspunkmg.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gmcdboscd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gfzenpkwh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/gmkcdrvvh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/geoobiwuc.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gxwrwykhm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/giklkpfht.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gtfzatlen.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gsykplwlg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gkuunkzsr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gccoqcocp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/gkkjqtyrc.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gceoempxu.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gbtphqfnc.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gudkususn.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gwqogmywn.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gngsujazj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gqrcgqeqc.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gmimhbbvt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gfjycqmuf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gcqwylnri.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gyayifzbz.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gktoqpnle.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gztwpfktl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/gtnonbpot.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyfjvxqud.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gmwybphfw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gosdamjoq.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gtxlnbkaw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gbbzjngve.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gjoiahtuv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gvuxivrfx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gtlqarqmz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gionngbwe.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/gqubyphne.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gwhvihflx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gtyhgulvg.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/gtvoaqxbq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gtktfaqli.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gpfnzrhxv.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/guouerdof.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gsfqorlhe.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gpbsrvauu.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/grxnuohss.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gmiyjbitd.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gclbyxleg.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/ghglszwpz.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gpwpbmhuk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/glxuwcomm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gotcjilnv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gqkjkhehy.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gmrxcctnc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/gabefcfwf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gbapjaqfm.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gwrjqpgsz.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gyikzjhij.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/guvgugamb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gqiiupziz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gykritrlf.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gklayvzul.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gectytqzr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gtlsmntoh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gseenquyz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gbdtlvolu.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/ggnukyszx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gdjrwfpdg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gdwiibmqz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gskkifjhm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/grfjyuolq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gsgeixnsy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gmetgflxp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gwvqpszih.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gsgaoqdqh.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/ghkagcmgt.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/geefowxzb.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gdxfydlar.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gflskmohk.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gxyxkzfez.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/genqcabxz.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gachdtpgl.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gagqlpvuz.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gzebmkuwg.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gtjxwkwem.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gpknuvwti.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/giymlkaae.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gcxwbaudt.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gnfldgfjq.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gtbeevwvy.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/gwfkdgwqs.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gmbrlmgyn.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gluzvaujv.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gfpafoown.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gvgqnotcp.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gpnstfouk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gqeibyiyb.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gigaqpaku.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gunluzdcp.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gdcycqcwl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/ghvkttcbo.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gelhvjrnr.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gqpajyiqe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gszweaqbd.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/geikvndhw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gbvgjpshu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/glbbgnjmm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gxnekxdqq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gqqepbkcx.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/ghtopfqol.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gkrbzzhmp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/geqoyisyd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gccuhpxzk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/ggyirlobc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gfrfixvrz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/galpgvbmb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gvbqfduiz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/ghtjnkspq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gogrddtof.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/ghijdrlzs.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gmsuxntbn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gboxjqqgf.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gbyjgxxfr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gwvhmxerw.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/ggruzndkl.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gfrycakxn.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/ggmzkkqgu.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gsirmleyn.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/grqfhpxoi.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gosflexrv.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/geskfhvnw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/glqlerzbu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gmedezndh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gucharfto.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gmqbigbvd.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gbfymalmi.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gneejldpo.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gpkswdhky.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gpjgplqcs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/grpaguxcy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/gggmvpzjt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/ghltiraib.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/ghbnhlyvp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gsqqevepa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gpetqqsiy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gctfqxieh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/glugngkte.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gmkjsibou.sHtML


<!-- 参考信息 -->