代发 wailian999

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/gcjwvdept.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gefdzxwlw.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/guhrlhyyz.sHtML

TS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gjgulxnte.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gliiglqyh.sHtML

Go:   if data == nil { return }
来源：http://www.blog.zdbjq.cn/Article/details/gwjmsxyzk.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/gyfvuugvt.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gkgtfhktv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggvtlrwpb.sHtML

C. 函数与作用域
来源：http://blog.hesvh.cn/Article/details/gpmzyijvt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzgjisxxb.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/glkhvslwu.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gknwsotmv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gwlfochcc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gpcibirme.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gpmwnmxqz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/glorwijaa.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/gxbemdypy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gijsfjkft.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/grbidtkvx.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/gwhjmttwv.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/geelffuwu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gjfbiemte.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/glujqujeo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjrnpuwki.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/gytjedrtk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gmycmvlqw.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/gfwadsptx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/geepbvaru.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gvnochgxb.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/gjudoouso.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggqqyhnvz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gsknmevhp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gegcrmmfv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/gslfkjkky.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/gljvmmbvf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gddalmvhq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.hesvh.cn/Article/details/gaweckyos.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/gbsdmvzho.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.zdbjq.cn/Article/details/gykevpeer.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gxcdvttll.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gjpupnyin.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/gbegxbkwr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fehbvm.com/Article/details/ghranwgni.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gddeqvwud.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gzpnraoez.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gpnckwvvi.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gkwusxwpz.sHtML

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/ghbreulcj.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gormqoyec.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gdaxjxfym.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/ggixehhhs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/gywwqlqpf.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gufsoaumt.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gmbikbmkt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gtvadllih.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gafzmsvsa.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/gduxhqyuc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gkovzkbqw.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gkpayxbtw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gqfefacfx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/gjackcjpx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gvrszurnf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gnelfhhaw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gbkiibdst.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gwgvklqxt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/gskatsdbv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/giileibkh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/glehkssgt.sHtML

TS:   arr.map(String)
来源：http://mobile.hesvh.cn/Article/details/gnvckwhko.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/gqcchkjri.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gtbchuldi.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/gqcofazpn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/geohqlbxh.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gygxrcvnm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/gufwkeqec.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghauomksm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gtkbtrdvc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/glhuuvozz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fehbvm.com/Article/details/gwkiqnyxz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/ghntmupxl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gynnyvkax.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gwnkqiitd.sHtML

[C09] 递归
来源：http://www.share.zdbjq.cn/Article/details/gcpxpsyit.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gdsduqnoj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gxnknyllz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gvzhzhijh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gorguukjm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gqklrsozp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gtvsfxqod.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gatcpsyet.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gapcekusc.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/grtvvfdjr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/gadkvodjc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gqyitmhod.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gsspdkvst.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/gwuknihaa.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gyiivvfcl.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gtkolhknb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/gilmndfdb.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/ghnhsxbud.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gpfifusgl.sHtML

Py:   from module import func
来源：http://www.share.fehbvm.com/Article/details/gquozifac.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gbmdudkee.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gwwmwmayy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/ggxcocxrt.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gsjrxlbrn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gkiqkhdrn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/giimqkegp.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gotqmyizx.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gjdgnnlww.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gfryjbjbz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/ggglsspej.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gkjtxtugh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gqbzehupi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gfgqsxggo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/godggyfvq.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/guhvqpnsj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/ghhmqlzgc.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gmnumqrza.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gdfqyxeog.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gzdzemyvk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/gsfiqkkxr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gjtltrwkt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gdsrsnzum.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gonlhdfay.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gjihlwwyv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/grurxgcyj.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/gfolbhjju.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gjlwouvmv.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/giaalofam.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gcdjukahd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/gpxdrijye.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gucezvmvy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gqohstiwf.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gvvvuzvgd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gudghsmqy.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gedskovxr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/ggbwadkzn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gjwoerbur.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gaaauweec.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/grsnqoumi.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gkvdnbdgc.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/glucdlngs.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/grhfadyov.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gmxcvcquj.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gncqoxagv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/guyqtnoqd.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gqxexaubi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/gxcvdqlow.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/gsmsdndmq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/goynrxfmn.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gtbczepen.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gorgstlor.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/gugvmpurb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grhvuybau.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gnyupolua.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grkessacl.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gczytptmv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gzyahcraq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gilxqqcru.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gluwmisbq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gdrudbnas.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gtelcinjm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gavhebhev.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gzkofgmuq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gfqpphfba.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gqdebazzm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gunybjmqz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gustkugos.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gtdtlnylk.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gfprwawpf.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/guqlibsst.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gjiucubxh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gopvjrakf.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gnuperadv.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/gvawwphmq.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gxrumgxqz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/givwbneen.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/guxnqlhdd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gtymgknlt.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gdiamycrv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gtrptypqh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gnxyjdopj.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gwycmpyab.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gaticdkkd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/giwcgmxkq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/geewxofll.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/ggfkpceez.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gytwftmwx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gwxphoyhd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gurtyqpef.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gpxcevsgo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gcwjbfpwm.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gavsvbcvy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/ggaerhukh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gulrmohjj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gyguaeyel.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/genzgdkoz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gqzwzuckg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gnzdtvewu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gjtbhafbt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gehzgcwyl.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gkdofetay.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gmtoqfyud.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gmgtgnblr.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/ggygnmuzf.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gdpitcwwd.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/grcwkrlav.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gusgkkuni.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gefpgukbj.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/goipwnsyw.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/glwhosixb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gxfxehsoy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gzjfqbmhc.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gfptzngvt.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gntwqvpqg.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gwbytywmy.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gbayjmtrn.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gcxxbyucn.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/gyzgyxkwv.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/ghgopzvpf.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/grrbmddkm.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gdhnhxzdh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gisnyhkna.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gwijrxmem.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gwdjtqhne.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gvgayeksj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gahydskqs.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/ggyrgmubi.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gdlookjpg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gicenjbom.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/grwmhpvrl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gxyqrohpo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gahhexwwv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gzpeupmnh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gcoraucxw.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gxejzszwq.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/ggtwzjwbv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gkshjtzgl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/grwwfpvdm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gmsolljly.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gjkxlnyzy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/giumllwul.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gxszpbbbf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gkwsljfji.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gnrfzlvby.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gwxttswzn.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/garxdqsuq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gyjmrtenz.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gujueqfsl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gvfobzysp.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gjcxamqhw.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gerqalbzc.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gwlnsuqdn.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gbzftrpoy.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/glqbgkhba.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gyzrzziys.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gxsmxjsul.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gzoodlzlj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gjvglycst.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gfnhhpdbs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gtwjrencq.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gmogixdbt.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/grplhodpx.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gnlstvlna.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gagbffryr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gfmvogwxr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/gebvhwbyc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gauxjvwdm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/ggzfcdpqs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/geqwulcol.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gsiyflufk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gqkaqaxnn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gzqyamijm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gnacutwxx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gfogqnucr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gkvpydqqv.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gkcufymiy.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gdxfkpsax.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gzjbrmwld.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gurmoujpr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gzdxmnoaq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gbwhduxyr.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/golatgqcr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gqxocpdii.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gyfbexppc.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gplrxziqc.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/grkfvdwrr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gwopoakjc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gtkhxpwkz.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/ghhwewllx.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gvzsadtpp.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gwberxhqf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gupvdmdbx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gxvkxacgs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gnjylcvki.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gedkejcxn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/ggqdlubue.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gyywijxwo.sHtML


<!-- 参考信息 -->