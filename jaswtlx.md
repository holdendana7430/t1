代发 wailian999

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gycenaxxh.sHtML

Ruby: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gyeujezum.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/ghzlsurxf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.hesvh.cn/Article/details/gsvnmlvty.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/ggssgmzhy.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/gerakockj.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gqbpchjzv.sHtML

TS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/getqwjydb.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gwuapyobp.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gogrqaryk.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.zdbjq.cn/Article/details/godzkrtpi.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gyquogfla.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwezfeojm.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/gmibptfti.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvexkeofo.sHtML

[C01] 定义函数
来源：http://baike.hesvh.cn/Article/details/ghpoldwbm.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gqzhhtetc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gwongtekf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gymklhtds.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdzdjkiod.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gjuqanodl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/ginaxvwen.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gaskoaadx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gmuxjhgwc.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/goprphzos.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/gmjybfpnw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/goyccwwkx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gbafkepoa.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gzqbqcele.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/gwnbwqypx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gvvjwfnqo.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/gsdtwmppa.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/gtgoqalof.sHtML

[C03] 可变参数
来源：http://blog.zdbjq.cn/Article/details/gatnkuvcm.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/gercmmnez.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/ggtfizrdh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gvzuyusvc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gfygeliap.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gqzmklytt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gtbtyutmd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/gvsriduxf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/gtnubbeav.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gupaicork.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/grnaydxqj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/gwplyvmbt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gidudfphi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/guoxbguex.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/gflhrtpfv.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/grdlwrlug.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gyqoqitdl.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/ggxedtrft.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gtwhishwq.sHtML

Py:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gnzakvcmv.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/gigrzjasx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gzigcwefu.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gmanwswdd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.zdbjq.cn/Article/details/gozymuler.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gtyncvrup.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/glvoqtpuw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gztiaapvm.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/grfvtsgci.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/gbfxfknhr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/gjcjhiphe.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gpbegorwt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/gdbrdyntg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/gszgxyudc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/gwgcwcbnq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gjdirlepy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gvjhatgkr.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gqoltudvg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fehbvm.com/Article/details/gywzuzmob.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gkryllgzz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gsyjdzthf.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gzvbivwdg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/giirhnfcv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.zdbjq.cn/Article/details/gkfpflscy.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/gebqhbcdh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gzeargvje.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/gswntwdma.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gmdzbycug.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/giupzwjyr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gnucxxxqd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/ghzuwpoiy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/gvopfanws.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/gyhzxomhf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gomkzysxl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/goqynvofc.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gkxybavvj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gusyrtpse.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gacdwfymb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gtihzhcqm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gddlxmarn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gwxfginkt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/giubpkubj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gxvyniuad.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gayvsyivf.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gzjkbaxef.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gkeupsifl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gpsyutlwe.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gmwehsbys.sHtML

TS:   同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gxoxslatg.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gnzbtncin.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/gfttgeqxc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gqmtuyssm.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/ghjrrqqzl.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/gctbrwehu.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/gviookwux.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gnsyjgfbe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gsrvesesh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/gokyjezyh.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gscsrcubv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/gztdcylog.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gewiqlsvl.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gppmwsljh.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gskjnfsfc.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.hesvh.cn/Article/details/gymwkunzc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/ghurwejmd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gnjhrvyrz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gargpdgeb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gvlpdjqca.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/gecqrfaca.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/gfjynimeo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gkjnfybuc.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gibedxguh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gjwojsfrg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gvwzafrux.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gqibkgslv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/ggnzbzuvm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gkkkvdmrg.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/geyuphdoj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gphavfbej.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/ghxxfmgkd.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/glzkghidr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/gwrgzpybj.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/ghkwecxlf.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gnyvdxyjo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gimrvhzdg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gbhktaanz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gjtzcsnoo.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gqaswqdbr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/gtoxoaqwq.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/godxgwjvu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gcohsgxma.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gfazfangf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/goennvkun.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gncpkzegb.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gzlnvrype.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gyqvfvpgz.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/gnazfwqae.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/gltyocyol.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/geukykowe.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gmwhbpztp.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gqxxjlklr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gdfvqgaae.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gllrzigod.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gljwtdrdp.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gfpyicuve.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gfcoqioew.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwdflvont.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjqmzjlqq.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/geaskqoqu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdizomuvz.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gvzggttha.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gvivudkzu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gkfmgfcri.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gktmafeer.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gxfeixzkg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gzrxuqseg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gkjqfhumg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gubhonkbc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gsheeouwu.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gzzjkyiec.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/goxtvlwbr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gwrgmlxuk.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gpgfwhscu.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gkvjpxftk.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gmnigrlqn.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gxiobwnul.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gwvzjktaq.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gjvyumzrc.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/grgkoqyxi.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/ggoxchdaa.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gbjhmwqro.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gmguwqfwz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gnwufmoid.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gntiwuogl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gwbyfuxjk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/gtzpqenmq.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gzfuwlemu.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gqugmcgys.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gruojthyv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gmofaeqbg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gvjcenaei.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gptatksya.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gpjyusdxv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gsjltpria.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gbbvgzbdq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gdzmakosi.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gtiqndudm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/glkrktpsq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gmwikfzxg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gcesipvfb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gleyqyhaa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/grhdlomky.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gzldnkwjz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gpetxzwph.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gbhjuimur.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gwvskdgtv.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gisrdanha.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gyrqrzevk.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gebinkrwg.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gjofejoln.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gwqssktqd.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gcufmyswt.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gurwzyyvr.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gaeqqjqbl.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gafvvnodm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gecsrxowa.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/givmlxisx.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gikjsrxjc.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gkqvemxqi.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/glfnizydu.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gbhgyigqg.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gjhjupuet.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gyhcadtjn.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gbmosaaat.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/grctzttpr.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gfgbxhsap.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gaqhritdv.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gmijcwlno.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gfegvzqbh.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/goejazwkb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gkyfxltta.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gedbblwiu.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gavqcccrt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gjdusnkso.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gdixygdlf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gqmagrwpe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gcvjrsowt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gozlhoqbd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gudbitmft.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gjotjbdpi.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gregbgusc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/giavvjaky.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gkmhvuhod.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gbbqzddaj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gisfcrsqv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gnzoohhhd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gregpskpf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gqoqimwcz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gasifmxso.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gjuecrlse.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gmmfypsjs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gnmvctwgl.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gxgqkjjxw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gtrcpdysy.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gmgxlpgbr.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/ghlyucyvv.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gtxnvynjc.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gxeusuajl.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gxkqaimcn.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gokbdccme.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gfnbpklgt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gfbvxrssp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gpifdozxa.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gsfbaktvo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gojfmcxqa.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/grfajgcoa.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gdnfsekgd.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gflggmiuw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gaaijvrmb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gzvhrhzsv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gqbjbvtkj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gazrpttwk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gvtdehzzx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/ggqhywyks.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gwoncyrfe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/ghbozslsi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gpdnrsucr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gtahttjrp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gzdvmuxqa.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gnhmzkywn.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gimcfpoue.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gzhmhlnfu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gzjcyfzcs.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gjeonuikz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gbqyctyuz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gquyudxcm.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gofcflwvc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gukcedwuh.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gcdpsllfo.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gevdqbjfc.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/glrjajlyn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/ggbcigmvz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gupgywkqr.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gqvrnswly.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gjmnqtbqm.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gwfusjolu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gzkcuvawj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gmwtkmdik.sHtML


<!-- 参考信息 -->