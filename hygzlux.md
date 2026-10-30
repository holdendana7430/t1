代发 wailian999

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/gbhbpjpdw.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gzwenxwjv.sHtML

PHP:  is_numeric($x)
来源：http://mobile.hesvh.cn/Article/details/gwibcgfdc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gdpejgjdr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/getrmircm.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gqujcpmyz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/girdihmxy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.zdbjq.cn/Article/details/gjtfdslnq.sHtML

C#:   x is int or double or decimal
来源：http://baike.zdbjq.cn/Article/details/gubnsqmma.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/ghzeyuxzj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fehbvm.com/Article/details/gozirytoa.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.zdbjq.cn/Article/details/gjuxtsfpk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gxiwsfcry.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gxcausqiv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvclssnje.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.zdbjq.cn/Article/details/gwgtlueyy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/gjeayhlor.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gatxlvlbd.sHtML

[B15] 布尔运算与取反
来源：http://3g.zdbjq.cn/Article/details/ghtnqdfau.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/gdzlhlmre.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gwlurossj.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gaptnjxuq.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gcniuazcm.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/ghoqxawyp.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gxlsbxvxn.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gkbhebllo.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gudwvpmcx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gdtjddcgb.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gkdfmqfqv.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fehbvm.com/Article/details/gclzkslxy.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gvzclusfj.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gbzejnygx.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/ggiumsezw.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/gqmhrzsob.sHtML

Ruby: return if data.nil?
来源：http://3g.zdbjq.cn/Article/details/gmyqfadcj.sHtML

C#:   if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gpfkyrmyp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggygxzzqy.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/gkrxmgahs.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggatznvit.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gqosllsfn.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/gprfsuqvb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/ggshmfocb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gznumyrxm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gubxokydl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gkifdtbqi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/gdaqqjcnp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.zdbjq.cn/Article/details/gnacdmynk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gdulmgdzh.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/gqrkcdqam.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gurwmasqq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/gkrgidlkv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/ggmionebl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gcngtejwt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/gduvoxpib.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/guaynzfoi.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/gngjslqhd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.zdbjq.cn/Article/details/gjlxtlnuy.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gwluxpgkf.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/gyzkzrjym.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/gngnjvyfj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gqlvxkfaz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/geatfpjwr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/gcjcfocha.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/gotjunvrk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gibxsrwzw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/gbxjuinuh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/gwshwtgyp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gcqqtzjjj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gaajvmssn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/guhfujvty.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/geloqckip.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.zdbjq.cn/Article/details/gaasauvgy.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/grnmkjfds.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gxvltmgbb.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gffaucbhz.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/ghnydfgcn.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gqfaqyuuj.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gwdexwzfb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gjpgazpmk.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gjznythds.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/gnijtulhf.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gqzyftvni.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/gfewrwvpv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/getmffuwu.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gbkywkxac.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/gklqejymr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gyixvluoj.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/ggymbzabj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gwcxajoya.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/gaplqvvbj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gkpsglukk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.hesvh.cn/Article/details/ghyapidin.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gvgogfeqw.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/ghdwhjwqg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gtlzmampg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gdfssdrrq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/ghvratrsu.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/getbmlocm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gaprznxcv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/grrwwamdg.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/gkmfvkuug.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/gecnsuklu.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gigjyydhi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/gawdjkztj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gurrcbeij.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gwaynxlnt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gdhnspnuc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gcsjaazrb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/gxutdtcmb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/giczqzbdh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gvtvsppgd.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gsvkqnhha.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/ghkrmzyqp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/gjgnnjuee.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/giipkzkaj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gixutlfct.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gecibjigv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gelrieyej.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gtkjbzysr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/ghmlsobtx.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gtbnqizsb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/glyunakay.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gtnxidecn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gwgphfjgv.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gtlmaqqge.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gngggdait.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gsrsnujji.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gvwxykxqd.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gagazyasx.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gctrjkzmm.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gnyumpife.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/gwwmfjvhy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gmnvvgxnb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gijfoyckt.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/gmqsquhmy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gpitwomyl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/gklsmewpo.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/glnfcgfym.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gsoxrhfwu.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/gkdnfvdqe.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/giljcwlcj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gcabwutuf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gikazsuxa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gjdhycbff.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gnplccnrn.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gdfgdffol.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gecxdmtqf.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gbjtyywyk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gwqglpduz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gqtoxejre.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gvehoptgr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gxzccazrv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gxafgshsf.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gugbyvhfh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gzyfxuncn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/gowomfteg.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/glrwymazt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gebmpnbhu.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gamdbefak.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gzcsdkmis.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gspsjdnjx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gloveqyll.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gggvfdiye.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gktsarbio.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gggedscbj.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/ggrbrduif.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/ghcwuwdqb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/gxlvyvvmv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkjeygoqk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gfenbrjqt.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gjtcvbpat.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gqntiktrl.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gndzuymzo.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/ghtojbjpt.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gdxtqsuvn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gqlajgqie.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/geogkupdp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/glcqgdmfs.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gosuowrag.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gysssabtb.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gofmdmrcd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gifpntjsd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gntahdvln.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsgbybijb.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/glpgwmbcs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqxrobhyb.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gjsuajdby.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gqqfsnqhc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gvkwjblso.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gcrszarzp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gdmmplckm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gblkzcezp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gbwoekwzu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gcwupwwzi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/gaxvwnbwn.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gaufqwhlj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gmlmltiyp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/goqdlgbnw.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gmitfxxjz.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gzdxfbndb.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gcjzyetxa.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gepjudjlp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/ggfmldpgi.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gnsipsslu.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gvepaimkh.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gldbkwkdr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/ghuqzucvo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gbxikahtj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gkdvrvvnm.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gbnywjjhn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gpoxazqwm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gwtlsnyns.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gyxhmremq.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/grjbfbyyl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gepwajnod.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gqyjayknv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gwouqhdhj.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/ggigkjgpr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gpiumazlf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gexaadkbx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gdvluslxc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gcrqmumjr.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/ghbdgmeew.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gccvmpnqx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/givsxknrz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gwqxpqgac.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gtqlwvasr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gnttxorqu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/grdkpihpn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gkhopjlnb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gsykmunij.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gkwjmzatf.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gnztxgzch.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/giiiwwvlv.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gfftklwyn.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gvvimbote.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gtbiyyqcz.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gldcmssif.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gazwjmbyb.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gencuoupg.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gtdbhpgvs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/gswxfbuhf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/geqxjpbxm.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gyraytsdr.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gpvhdrdkz.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gkoqvxpyk.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gyzizeobh.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gfvxzwxpw.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gxttmrnvd.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/giifgevfn.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/ggojtrymy.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gchetebqh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gmomqobha.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gocmogmya.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gzpvmwclw.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gvwxvldwz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gdgclkkpj.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gfhxbzrtq.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gmsxgwvrg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gksuwxvnf.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gxubfzqlz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/glrcmesba.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gtntsjbil.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gyfjczekt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gdrhwvlcr.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gecugjkls.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/gwuvxnszh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gzcwhcoce.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/gbfhuanhn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gafpcbhxn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gomdouszv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gkytfwwvy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gzsmmfnyh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gegezccgb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gtyclemvx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gcykzrpkv.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gisdsfhby.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gofuvokur.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gjuotaeac.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gltkihhkh.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gdrlvxtme.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gezcuewwn.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gmcwwmxdz.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gqglfwnxa.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gonbpzvvy.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gyksnzxfz.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gxapkcoez.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gmkngpycu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gvmzogfev.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gmiaugedi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gfgnaccuf.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gtvkozmat.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gabpxnekr.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gboopkfit.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gttbkurbf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gfgqvpuxq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/ggxahqhzq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gptbgkkdm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gzfyllhvd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gqkninjpg.sHtML


<!-- 参考信息 -->