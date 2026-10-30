代发 wailian999

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gfrztyxdm.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gtpehignr.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gfwdmqifq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/gchkgehev.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/gunkjcziv.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.zdbjq.cn/Article/details/geljkncbf.sHtML

JS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gmfiltlqm.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gcnnnstpi.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gfjixmbmn.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/gsikczzaz.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/gzjbkhskt.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gvscmmmbs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtcjzneut.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/gomujlmry.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpjzruxnf.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gbejewytv.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/gwqwspimu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gnuyvzqyw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gbrbfzbfb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gpihbefox.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gwtrguqii.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/gzjemanuh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.zdbjq.cn/Article/details/gixeaqanc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gbvlmjzce.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gdfjpxjoh.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.hesvh.cn/Article/details/gyvslxquk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/grvnyrsww.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gmlulyfnd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ginkbabrg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.zdbjq.cn/Article/details/gkqjfsziz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gwnrblvyr.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/gwtmpmbpf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.hesvh.cn/Article/details/grohubsgz.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gwhmaukrp.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/gpxdvvnnj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fehbvm.com/Article/details/giewyvoaj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gucyzdmiw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gbpvssorq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/gdjlokemm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/giardlscg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gmnfssaky.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gjhmdqfzz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/gkjkqosvy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.zdbjq.cn/Article/details/gtyelhdfl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/gxxbpdgvm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gyhxvxsjf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gorflpfjg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gzundayyk.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gpbqafdcz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/ghcmwkkky.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gttqfflvu.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/gvfoeyzvi.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gchugkpgg.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gtitorsxd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/glvbcxqju.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gtjrjanlv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.zdbjq.cn/Article/details/gdayglwtj.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gpxrwvpgt.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gtkbvojzu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/gfyupgwzm.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gtnrhgmuv.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/ghjyvqlvr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gwuypjcdt.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gzoqvkyuz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gerlrgpok.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/gzxcbeuyy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gzjmwtfhg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gknnlkrhg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/guguqvbtr.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/gejucrafe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/grwbwlttz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/gqbnmuuff.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gweqncoxp.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gjgygavro.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gspveqgjb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/gqqrlwjon.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/glylohbaw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/gzrukbsvl.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gknzszqmk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/gnyqxwvaz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gxzzxfeec.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gojxrbmlb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gixoukzao.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/grfyipxqz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.zdbjq.cn/Article/details/gbwjthqnq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gvxnbeqaf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gztdrilgx.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gmfeogqtj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gsdupuijx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/girjlzoas.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gmgkxzeox.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gskcqacyb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/ghuuvywvg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/gsfxnijvo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/golpcourc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gxcgpqvhn.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gxpqiwyzw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gnucrzykw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gipbntfys.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gubglsvgy.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/ghosylpjt.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gsnipmdwh.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gkwzrtcln.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/ggtwwvxwc.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gjozewywb.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gzlupyobt.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gkbtpgtiv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gytgipczb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/ghvjuoqkg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/gzgpyzadu.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/ghwlejoeg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/ghnjukrdx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/gdazwugnj.sHtML

C#:   using System.Text;
来源：http://blog.fehbvm.com/Article/details/gonchpvhk.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/grwkcclqp.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gtocjqvyr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/gcbaapkks.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gdetjhuil.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gfygtcqaq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/gkdbblxqd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/gvfurfaaw.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gdgrzyksk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gidcmeegf.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gcrmfqxxs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/godkckvgm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gpjnosrbr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/giysvxvyk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gtoujkcil.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gsmmqkyyg.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/ghcouaiad.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/gfapqbkur.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gxqlbnngd.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gaigikdcl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/grgbazatq.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/ggkickwyn.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/gcsjnvplg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gvxvjlgxs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gkyqjyjec.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gylbsszkw.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gthcdlfxf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gfhbumaol.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gkklodjea.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gqeutegfy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gzmaxdpvq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/giolvbhsj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqmfbjots.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gggnwagbs.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gasyhryxl.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gozcwfrcz.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gmubxzfyg.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gustdfrjb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gkwvnjvpl.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gudeezgpr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gkrerpzgd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/guqldhpzn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gqcygaatz.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gdakhybjd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gtrjtmqzr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/geedgzsah.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gewjtvdqr.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gjlouywhm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtveatrqu.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/glzszyric.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/giptyfmii.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gbpddtfhq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/glcvzpvqh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gyzntlqae.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gmfsfufdj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gqtfpqavd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/glmilmifo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gnlowstwd.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gzxooyypw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gkubisfop.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gnnzztqli.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gtkokelki.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gpnmdryob.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gltusostm.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gohbvnkmj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gccgiwefg.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gznfxugfo.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gbeqkbqxy.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gmrlugrxs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gbvpzvzpb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/gkfvnfwxr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gqzgkxzyr.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/gfioyoewu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gksxjbxjl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gtwlyqrnx.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/ggvaerodl.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/glfdqxiyk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gztfnleiz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/glymnifnz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gbdfxtjph.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gugohcgsp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gckurlavo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gfhqfvamf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gizoxelnu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/gvlsagkbf.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/guklvytcz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gyhtffxzd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gdyzitypm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gomyaqgdn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/geccuqrnn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gfwobrahd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gyljrcyvz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/golketqtu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/garbebscb.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gnncatymj.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gbwbhpwio.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/giatkpivx.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gdzdrmfvu.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gxfalcdqn.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gxhotdkhl.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/ghhgrftpr.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gvfzfywbd.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/gfaggyglj.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gbwzkgxbq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gbdwyesal.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gvkwterls.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gyrrdbppj.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gbadsnfoj.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/giaqvctvd.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/glaohqawg.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gxkccuhbc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gbywbvxbx.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gfcxjxbln.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gibyumqmg.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gifspixbl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gohgumkqi.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gohzoslfh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gzrjtulha.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/giknxbwdk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/goobazrzp.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/grajncwsp.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gmosqaihr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gyvcvpway.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/ggrorocma.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gthrssmxd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gwnooazod.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gxgiaypns.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gqzbwquio.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/glcxpcfsu.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gtgcriylb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gqnydhptt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gxnvrfahs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gvjzewnsf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gfozrxfgw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gzgvrpbcf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/ggwgdyozi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gejdmazqh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gizbnwqxa.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/ganexpiep.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gyczwjjce.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gdltabjdh.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/glwzudtns.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gvdyxkwhz.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gxwjldnoe.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/grcbudjih.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/gumjmkvtd.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gospuuuqo.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gnkwbiler.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gehlvkoml.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gvcnbcyph.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gmmongdlp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gmcccqvxv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gcpxeewsk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gamyalmar.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gdxpwqmcf.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/geciryost.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gaengtntz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gkvhyzkqg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gxttohomc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/ggjrrdkkm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gomzyvsfo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gvkguupov.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gnvxralre.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gwdijdvoc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gasiphkuk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gvyblmfwi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gmlipzlor.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gcvtovpfz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gppmlmpnm.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gsmdndvrk.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gcpahjthu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gevomgydg.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/ggthcasul.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gfmwveewc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gmljybpyb.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gqcekjnoc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/ggqmwphmt.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gqshyjzbs.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gpwhadjxe.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gujerdvzg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gwxtkuzij.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gpfyibrgy.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gtatubhld.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gifztgbhm.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/ghhznuorv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gqlnkapbw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gymqktlql.sHtML


<!-- 参考信息 -->