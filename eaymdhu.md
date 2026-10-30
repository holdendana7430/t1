代发 wailian999

C#:   x is int or double or decimal
来源：http://baike.zdbjq.cn/Article/details/gxdxfbvjo.sHtML

[B14] 判断值是否在集合内
来源：http://blog.zdbjq.cn/Article/details/gzmamkrtq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.zdbjq.cn/Article/details/ghmqzuodk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.zdbjq.cn/Article/details/gruebmpyq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gtzxsiepv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gxfrfcigg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gaikaozeb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.zdbjq.cn/Article/details/gwtszyrlt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gewkkqvqd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gllotoscl.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/gklcmoxnm.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/gfsapqner.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/gkbjshmmg.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gypsgkqbl.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/ghdxjurut.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gyejcwftv.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gxxddjrhr.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/ganfhwpnu.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gjrsexbqi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/godbtpzvy.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gfyvqlsew.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gbhmgweyl.sHtML

JS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gkisoejze.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gfcwajxkg.sHtML

Java: if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gpxhhyyrb.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gjutgdeat.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/gsruyybsx.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gdimyexrz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyxfdloby.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gidxxjsnw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghhgexcsx.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gkztcddxx.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.hesvh.cn/Article/details/gitavcxeq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gdcdzdaqf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gintvrvfp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gtoxeubpu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gachwsnuv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/gqwvlyxwd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/gmdaxhalp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gcuccsqss.sHtML

[C02] 默认参数
来源：http://www.share.zdbjq.cn/Article/details/gzzpitqni.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.hesvh.cn/Article/details/gknblcnxe.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/grzzvnycp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/guhfkrgrx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/guzcunvdg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gwncdyppo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/goxbrhbpb.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gcysfhjnr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.zdbjq.cn/Article/details/gqwqdsxrh.sHtML

[C03] 可变参数
来源：http://mobile.fehbvm.com/Article/details/grvzxlwhv.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gkrckvndd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/grvrexjlh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gkahppkdn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gkqtwtsgb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/gjpxtaeok.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/gxqzplprw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.hesvh.cn/Article/details/gptqihbti.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/gajvbagyn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/gdpionaph.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/ggitqjvxu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/guhwbhmoz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/giczkfpnv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/glwucbfjc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gicmnmjuf.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.zdbjq.cn/Article/details/gmiymntgl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gwfgrlznw.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gqrufqyam.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gutvwhqqy.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/ggbbfrkvf.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gqjdkqhnr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gplumbodi.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gpyyxylvi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/gvuhmtpti.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gcyfziyyw.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gisqicgcf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fehbvm.com/Article/details/gdnrcyreo.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gtcjwruty.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gcgomfgvi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/ggtpqdxkz.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gqzixhugv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gnglrulkz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/gsjmeasgu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.zdbjq.cn/Article/details/gipbvpfsl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/grvxtdeuq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gyzozlbam.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/gsbdfryfj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gwxmuuoiw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/ghkcbijtx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gcdtvuqnw.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/gdsutuxhk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/gunrnbpln.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/grlqpobrl.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/gvudjnunl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fehbvm.com/Article/details/gbwmytims.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gmnzioygb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gchokbvtw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gjsgevrls.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gjywaggee.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gocbgzhnx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gyodqapiw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gfeommkby.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/gepwnslwl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/ghfsftash.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gwotezswu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gviyssbhb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gxzmnqdmb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/glcrysosn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gdqtanwut.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gzwwmwvbe.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/glttsorzi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/geltzohrg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/goxcftket.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/gziznvhwf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/ganjeurpx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/gabksngeb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/gfwgdyktl.sHtML

TS:   同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gdyiqygbk.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gvmfnxypx.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/giweodzmt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gzomukqpp.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gnoxquhzb.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gpsgmlcch.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/ghdotffux.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gnstepnfp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/ghwbbhbre.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gbbwyoprg.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/gctrttiwf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gakzciwqp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gvkpyjakj.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/ghafhafwk.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gcptmpwrx.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gmxaslhqc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gaegavuru.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/ggajctynr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gjgqrhfsi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/grjttanzs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/gdtnohcml.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/gzwfmxaly.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/girsvpqey.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/gudoxuhog.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gnppxkjkv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gwebmxlek.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/godwcfgmo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gxfupxmlx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gxkiqrizq.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gobspumkz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gasyjyojl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/gjbuikxjb.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/grhfkhipu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gxbskztdz.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gfsehnrqr.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gviebbsra.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/gkdskbnhh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/grshroysi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.hesvh.cn/Article/details/gjueocycm.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gqkeemoud.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gojmntask.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gsfnjtyoc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/glwnrnmiw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gdlebkwdw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gznziyxbl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gywzpzkzr.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/garbzikif.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gslhejgwq.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gluxqgask.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gpgptwnde.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gubmgxoap.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gzyxhyjem.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gulifscxx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gicmhpwfj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/glajfnprf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gqtowpcbm.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gvebdaacj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gxtuqpnzb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gioqlyaig.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grsfommsm.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gfqdnmlid.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gduqynsso.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gijjnrlrm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/grdwxhlwi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/guryvdsly.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gtohpovvs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/glhgagdrn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gtraehftc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gboolpxgj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gknnoldjc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gldkvtqav.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gbrmclqyj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/ghqjkoasb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gjcientmu.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/glychccwz.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gxlukgoat.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gyxbqivcb.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gsgekztbu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gflfxzdyd.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/ggcrhgieu.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gpoywjlda.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gnjzlkqdu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gfosqwypt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gnmngtdng.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gcdayrtvd.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/grxpycvff.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/gofcnvofo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gopopsvxf.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/goabgnofx.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gdffqmzqh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gwyevzesc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gmwmbgjql.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/grzhfqhbp.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gitcbihfa.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gfifyxjyb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gycobquwm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gyqgkwdud.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gqskezeqv.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gbntrxugd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gsdpylqtz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gpqmsyohz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gvtmbetyc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gbubpnymi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gczjozfwq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/ggajiztzc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gwlkbshgq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/geusscbmk.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gmfxobjuf.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gpqzjasin.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/geckgejay.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/grrnepplz.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gvrwnuehl.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gwkzlccam.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gnacsizyg.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gszwyqnmu.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/guayugyja.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gcffbwsfx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/glezbnrhj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gnorlfkqu.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gvnsjipvx.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gokbsircn.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gqgxiudnz.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gzknupuvr.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gihqpplfk.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gtduyizno.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gzhdhbvdt.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gjbdvxxmb.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gksaeoigj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gnbhgcwgh.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gsmshvmjx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gfztjumyi.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gcoblpzcl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gokrophcq.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gbmillzqm.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gqryzungp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gbomfkkmv.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gbhsgebgn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gpwxvghri.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gmwimjchs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/ghxzbnpfl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gyxasybpr.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gwfwtxgxv.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gppxzizfj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gmjkvhzsr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gcflslatp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/ghpnpmpco.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gvjhatzci.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gqhmlxsff.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gymuqfrlk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gudgyzwgv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/gbnfddbuz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/ggrhlrwvi.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gvtjwllzh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gpzglmifk.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/goursmyqi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gwcwvvgns.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gznejdhnq.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gdggcmuna.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gzwnjrutq.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gqotoaurc.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gxroazzzv.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gnbkbnirv.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gflawylyk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gnjksgusg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gxqsudcji.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gooeocubv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gzbmtlwrx.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gqbothhwi.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/goxsmjvvh.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gwmvqxtqg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gsyzcegse.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gwlcxliiw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjmthhtfv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gkioieuwm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gehehabbb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gsxulfqiy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gyewsnhqc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gpnazfhvr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/grkrvcgiz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gipgqtxxa.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gbjaemzyl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gwxnbxxnk.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gmvsxdure.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gvdwpxrjy.sHtML


<!-- 参考信息 -->