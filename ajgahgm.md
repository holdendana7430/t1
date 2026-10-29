代发 wailian999

Go:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gmbjmoqfm.sHtML

Ruby: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gncyvrlkv.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/ggivqzmzc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/gplbptdwb.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/ghypsjqfq.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gqcatyspg.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gvktcfgyp.sHtML

TS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/ghrzenfva.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gppndtgnf.sHtML

Go:   if data == nil { return }
来源：http://read.share.zdbjq.cn/Article/details/ggogfdeku.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/gmmvtckob.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gysgccqoa.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnuvhudnk.sHtML

C. 函数与作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gybjdneji.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjzxcaytp.sHtML

[C01] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gtatvtcsa.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gngperktn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gicvwbpmh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gsyedpaue.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gvrampmiy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gtfigpsco.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gqxykaexn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/giqfxtdls.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gtqqlvedu.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gzzomsssx.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gldfbnhbe.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/gnkzmkigr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gkkyiiyqt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gsvukjubz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gvjxxhjrn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fehbvm.com/Article/details/gbcfbegya.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gyvgfjwij.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/genyubxhf.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gkmuxhvag.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.zdbjq.cn/Article/details/gpmksxaeq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/gyhmhkqhj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gwhapezdo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/goorukiye.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/gvabjecdf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gxrptywqb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gfzpkiilr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gxcriwwgh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/gcihjmxlb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/gmcvbkgqo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/gaqsuqxaj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gzjnlpjqp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gpzyczeca.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/ggiithqcb.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/guebiipyk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/ggzrnnqip.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gdtmvppxj.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/gwuvqkwsx.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gqkmapnir.sHtML

PHP:  return [$a, $b];
来源：http://www.share.hesvh.cn/Article/details/gfoafqoes.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fehbvm.com/Article/details/gnbeyavro.sHtML

TS:   return { a, b };
来源：http://wap.hesvh.cn/Article/details/gyzmexmkm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/gkjmxzuge.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/geaaopgsk.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/goqieawyx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/gqmpqkphk.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/gtgsuznzz.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/guoptgbsk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gmvebqwmj.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gynnfuutz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/gimygoagm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/gxybykyxd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.zdbjq.cn/Article/details/gfxywhxno.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gyirqqzvb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gaizqxeqn.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/gbbihrfib.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/gonmvnmct.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/ggsbzuuhj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.zdbjq.cn/Article/details/gzlssvjdi.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gvofkvyrg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gbnjsrqux.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/gpidvztua.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/gqlbcedmr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gopqdrbby.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/gwrxyxtwe.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/grgdpkmlw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gmuovjavs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gdwwpjlky.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/glbeifabl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/ghdltpuyb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/getiynzcq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/gshiwkrbz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gevxtguwp.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/gjsbknzky.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gwgexqfjc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gkkrjmyzi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gdpbjoajl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gqdwrbovj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gvcqlcekb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/giwvsplap.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gbilfisvv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/gqygfnmjq.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/ggrvfkedy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/gvednkhsl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/gnykhouem.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gzmuxduce.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gzjbjrnea.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gjjvtxstw.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gnburtubp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gahsgllfe.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/gprfxsqmh.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/gurcjdzmo.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gbndqesck.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gfestvmgc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/ggjvrwxqr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/ghifxghus.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/gdxwrgvni.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gnswlcsab.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gkarojtng.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/gldsnjxcq.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.hesvh.cn/Article/details/gomubgkwu.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gzlevpmql.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gspkukcho.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gkcbzueqh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gfzihfauf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gicczuxib.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gavuctjzh.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/ggbwepege.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/grzcbopvm.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gdtkhedya.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/glgkatvmd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gjjrymjlc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/grkkizwam.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/ghjxujcbt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gbdmjethu.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/ghdlmzgbm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gohhzbfsj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/golhtqxvk.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gxojkharj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/goizvtluo.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/geloottyr.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gpzraasbv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gdntjlmol.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/ghlpqkvcx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gzidgjeqo.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/grwypemdm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/ghthbgyod.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gqctftvon.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gdunuwgrt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gdjpjblcp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gcusmzobr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gbljrmpxy.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gqwpqopbz.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gtadbxhhi.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/ghtsboxex.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/gycfojjrm.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/gdepgkxut.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gcyeyobel.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gpytvixqd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gctznoowa.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/gqwqiejmy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gooddahry.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gpsmgziem.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gnhdoqjwq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/gepgtekgg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqunredxk.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gagbnxuza.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfnxtjupj.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/geibctsji.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gsqgkztev.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gfqgugejj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/goelntdzc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gqhmilisw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gtwkthccr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gtlkqxgls.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/guyaezcvf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gqoxjflsr.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gwasyczqi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gsoaabesq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gavuuwkfx.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gfcbgexcb.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/guebmagdc.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gtzttnmjg.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gwufwkqkm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gilwgpwga.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gcozjfnbj.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gluspidyi.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gkcdgooyf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/glpohpcxj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gjnkgqvzk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gaesivdcx.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/ghimosaqd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gsgjtbdqf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gvmitvqlq.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gyeqilwci.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gcjjvcdij.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gwejbqltl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ghgtktgvf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gyqzzjwdm.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gukstlwya.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gqecxcnjp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gobjbluka.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gpastdjps.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gxoxeevcf.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gwvsktltb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/guazlqior.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/grwjohttj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gpycqikvb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/ghywcypah.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gmtvqnbjq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gcsgamrvh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gigrifray.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gqqsffnbm.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/govqglaje.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/ggvziqgjp.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gcuxvqisz.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gmapzmomy.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gwktdpfpv.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/glxfmlhah.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gcgoisxlk.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gvbsmlnbo.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/glphrcdxd.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gsvujogsj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gqmchtdeu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gmogjmqxt.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/glxctlydp.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gphulvewf.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gspuctrzm.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/giwwzyngt.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gaksuywen.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gejabcdja.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gkebuaqdm.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gtouwmqqg.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/glawqpeml.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gknzkvuyp.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gvwdwlhik.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gucndnhwi.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/ghausjrok.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/grypztrli.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gsrsgcxll.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gmtyqjlme.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gfwqtnkpp.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/ggqskhxmy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gfhjzsqyz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gjjllxqxz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/ghffkpjeq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gufrsrage.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gksxttaht.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gkuxtttxv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/giygkzifb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gxvbkkxmw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/ggrionhie.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gchgixiar.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gkzgkoqvd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gquhpjani.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gkmnmnewx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gqmohdtxr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gzcmyxcxy.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/geejgqxer.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/giotimzmv.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gdluhjdoo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gbqwipyjh.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gllqoxqye.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gxdjnalwp.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gwnsokgaf.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gvalnkmdv.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gcwnecepk.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gwqrferqw.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gmxuxkxyy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gfqvcanew.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gcbvgryyq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gugubpnmg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gdwoxtpza.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ghplymmjt.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gtcbainjs.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gstamzchg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gieigvhno.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/geufryugl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gyikuimvj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gwbdeaglc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gbgqvdndg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gxpsioilf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gpwhkysed.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gicjzsmrl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gqtnckjcb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gsbwnufbr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/ghyvgexyl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/ghdvqgtpt.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gcpilnspm.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/godnztipr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/ggomnhyqw.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gomaznfnr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gsuepaafx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gdijvfkgr.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gkzamoxed.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gmjzobjsn.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gokjnlasj.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gmembpdpp.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gboakslis.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gpciroqrq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gjbupmtit.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/ggymagkyq.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gsqjoxuag.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gfsfjsmnf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/gilqcamzr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gzwmugkmm.sHtML


<!-- 参考信息 -->