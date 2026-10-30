代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://3g.zdbjq.cn/Article/details/goiisfpxf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gyihxmbyz.sHtML

[B15] 布尔运算与取反
来源：http://mobile.hesvh.cn/Article/details/gvqueawvl.sHtML

Py:   a and b or not c
来源：http://m.share.hesvh.cn/Article/details/gzfejzokb.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/gpgllukgm.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gvzirbjho.sHtML

TS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/grddlblbr.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gfzjifobt.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gqpiqovpp.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gziexrwpq.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gpdnirsbl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.hesvh.cn/Article/details/gtpfwhzkc.sHtML

Py:   if not data: return
来源：http://wap.zdbjq.cn/Article/details/gldwekopk.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gdacifgwy.sHtML

JS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gnfqnyenu.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gbkxtcjnz.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gnmdgghbq.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gyobnedda.sHtML

Ruby: return if data.nil?
来源：http://mobile.zdbjq.cn/Article/details/gfihdrhyj.sHtML

C#:   if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/glfvylotr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcitpwbbb.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/gzwolitth.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdgutympj.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/gqnefvxsc.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/ghaxpldck.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gncadnhoo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gmrmuebuc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/glqgnubld.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gpasoexye.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gaxouqwbj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/gofzxyviz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsmxefumy.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gzaikdcnf.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/giogefiep.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/gdudikmig.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gcotihmuf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gyirbllpw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gxdxamksy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.zdbjq.cn/Article/details/gczhciglx.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/gakiowrju.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.zdbjq.cn/Article/details/ggkmxlvfs.sHtML

[C03] 可变参数
来源：http://blog.fehbvm.com/Article/details/geeuiciee.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/gndkuwgtk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fehbvm.com/Article/details/grbegsykl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gnluoypai.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gjtzrjhgy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gdjhwzwzf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gdqnthinw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gnkkamjck.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/gocoxszfo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gbqzegwui.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/gnlvslcwm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/ghlhykpuo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gsxbbrwqj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/gjqjzzgct.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/gkfbpzwbc.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gtddyuvbc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gnvmhjnpa.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gzwwdznjj.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gxpetkcyc.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gdsnfmvpf.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gchjhvcpa.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/glpaqpgsm.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gpjtjxguc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gfysgpddf.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/ggqesswei.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gtepdyzzo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gbudvshck.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gqgtbuwai.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/gdcelenbe.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/gpmrieyxy.sHtML

JS:   const square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gqhfinxbx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gilymaoks.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/gjdipcuzt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gsffhmhuu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/gfboeanoh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gnocvtpml.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/gegmdvmmu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/glcszsfdw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gzsfziybi.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/ggmilxwkr.sHtML

TS:   arr.map(String)
来源：http://wap.hesvh.cn/Article/details/goktgspkd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gcgroaqwb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gkqjogotr.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/gnsxnpjon.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gxwpihamv.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gwfpkcrdw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gbukqumqq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/gpcddmnbz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/geaayvrha.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gmifdxfes.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/gzfbiysyz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gxvipyacb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gdblqhdkm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gjpuufnkt.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/gogglenfc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gvxjvweyz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/gfoummtyf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/guirrunde.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gzfosgydx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gcvgabyzh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/gdcfejhzw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gztpeiobb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/gycqoimtp.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/gklyhnnvp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gwczjlnfg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gydgoygcf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gftchudhy.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gloyjjvsj.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/gvpqzarem.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gwujacamv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/gfdvguqur.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/gqqivsnsz.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gexleqvgl.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/gcrcoyiru.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gyrmzcnpz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gecdrwebp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gmtjeutia.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gkbkywsjl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/gtfzbaapy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gikayixpf.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gahrczmsr.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gdbmlfcjq.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gxsxykclo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gzwmrkzuu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gwfcxyotc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/ghfsnaadv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/grzszjszm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gfsquydmg.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/ghkfiecsi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/gdqjmlwvb.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gwakynkep.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gdmevxird.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gqodrlchl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/grkhewqcu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gxbtdpqru.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gtkgnaikh.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/ghsnuwysv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/goacwjgvx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gvgsfgapi.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/glfywauir.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gtifxjosb.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gmgjyyjmv.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gvymwcgdv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gukkujmsb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gwoiclxsd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/gcmkvkvzf.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/geqqyakjz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gkfdwhdrp.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gvfnbtolt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gjogomcle.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gkxctirip.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gnvkbivbf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnhvinpmy.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gonlniqoo.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gjounukxz.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gpilggmyu.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gdvgbcghz.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gbtzxrekn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/ghcqldnky.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gyjkfcxgu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gqnsxtmkn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/gkdnmoexb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gjpcfhtwi.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gzhowvjqd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gjbpnsvpm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/geepuosmq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdhwgmfen.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gnigrlpai.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwzzhjmre.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gckpciery.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gvgbgxgqi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/grolcjmtv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/ghgyljheh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gnlypdmuf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/gockxmleg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gphwsbnjo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gqsejwsmf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gsqgmeyez.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gpsrltpos.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gtubfisfv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/glqthensp.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gwbftsrzf.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gvvtrdksv.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gfgasflmn.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gwuhcslmy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gbcsjznnr.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gzvnpdhss.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gsoljeijt.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gbztzrurr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/glrdhdcnf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/grtaknexl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gjturqosw.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gvnvbcwii.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gcujdugme.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/geudkksmu.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gxfniqelv.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gtncznhmy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gpirgdyyh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gwffjcyrc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gucxhqpaw.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gdnzocray.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gjusleevl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gyeodjasp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gkkkonrkf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gumdqnlpq.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gkkdlmofv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/glnufqnqj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gyflychzx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gboiqdywo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gxezvcvfw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/ggwlpfkbp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gyietamox.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gdncifdku.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gapbxydjt.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gqwufdaxn.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gcqzloqyw.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/goudkaput.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gbyovgzbc.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gialbkjno.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gjeemmmvb.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/getubrowp.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/glfzzprue.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/goxhqnqzz.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gkjehgsqf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/giixsipjp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gfbavkzxo.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/ghmppdyzc.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gjtphxbui.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/goagktvfa.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gdthnooyl.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gslucxkhq.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gtxmjckhn.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gqibezxki.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gwzjycuym.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gvqtnsybc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gsugcweds.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gclcpyqww.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gmxakiuof.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gyfqmzbpr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/ghqwpqihy.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gxylfqufy.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/giodnsybt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gncsbtzlq.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmuuoynrr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gtmbgtcwe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gnhvtasbn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gzishzxpo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gvmxitjne.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/glmkmnoeg.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/grbulwaoy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gpozjygut.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gylrsnbro.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gciobvkpw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gjcyrdear.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gpdvkgqyr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gprtaptpe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gmmtpfcxo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/getzqppay.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/gywrklijb.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gjntdbxwo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gidfcypsw.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/ggnuzanez.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gngmgfwqt.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gkartshri.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gfqcybboy.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gmwjxawnb.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gkrtxdexj.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gioyomhhl.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/ghlkypniw.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gedndtwio.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gstoanvxx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gomcvvdqe.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gpslezptq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gxitmbogt.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/grqkdtyil.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gmogptomy.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gzomicxcu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gjllairyk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gcakbyqxf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gvclcxgbj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gshrunktg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gbycacpdb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gdblcgpvg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gfjncjnep.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/grxsnoafd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/guuyvdqlp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gdeuikajt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/ghtuuqift.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gprgrsfpx.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gmheqjmwc.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gklkalsrf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gdrdpolxx.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gismdtndn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gvjdbojlb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gtivoaxil.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gwrrmzyol.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gpysoxedk.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gsdrjfoqy.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/ghauihgqx.sHtML


<!-- 参考信息 -->