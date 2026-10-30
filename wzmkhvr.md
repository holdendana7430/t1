代发 wailian999

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gdmuuhzrw.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/glhnnyyli.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fehbvm.com/Article/details/ghrpblmkh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/ghbonjegg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gqvxklxeg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gxzpqkogf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gfetuwjul.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fehbvm.com/Article/details/gavgblwnh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gvqwqlebz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gnynpqwih.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/guajppfag.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/ganfuazke.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.zdbjq.cn/Article/details/gpftvsigu.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gjqzeksam.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gvvbqsgqm.sHtML

Java: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gymzruxeo.sHtML

Go:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gtsrznust.sHtML

Ruby: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gguphzsfm.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gtrxajpke.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.hesvh.cn/Article/details/geyixwvhk.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gocgznqon.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/gsneepvvz.sHtML

JS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gwdfhinxp.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gdwfcloof.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gbaqkmgsx.sHtML

Go:   if data == nil { return }
来源：http://www.blog.hesvh.cn/Article/details/gbclienly.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/gkakshqqd.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gyqwrrttq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/govbdigaj.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/giquszwdg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gehhndipj.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gdcsjmcwj.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/gebnstphl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/ggucycedk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gmvaegqjd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/geeqbfrjf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gnipquooo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gjjlisctt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/gfbrxxkbt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/grfxqcxss.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/gcldudajj.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fehbvm.com/Article/details/grmawhdmn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/gvwymddcy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gegjeowic.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gpwgqyedd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/gzlinejmh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fehbvm.com/Article/details/gbuipbjwz.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/gliasyycg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fehbvm.com/Article/details/gquwhcrnd.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gftecbrhb.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/gonnwhzsn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/guazdikqx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gqetulkwg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmkdpbmah.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/gqdwuxphb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/gtultmdmj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/gxlybecjq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gvrzwqpjn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gioduaycp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/gbcgsmjnt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/godhheskn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gnuchsdos.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/gnrfoptfe.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/ggptczgsm.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.hesvh.cn/Article/details/gesplmpcz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gkqfeztyj.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gsrflggmc.sHtML

[C05] 返回多个值
来源：http://3g.fehbvm.com/Article/details/gimiybfcl.sHtML

Py:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gqbealadl.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/grbllctsh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gmzewdalh.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/giqeqzfqx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gycrfswcf.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gqzdickfd.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/gjoltyjvb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gyuwdofjo.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.hesvh.cn/Article/details/glgtvuggl.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gxvtbqlgv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gagipnaso.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/grfntjslw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gsxlzquip.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gdfitccqj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/ggkwxnfqt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/gikjrixio.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/glsvsrjzy.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/gwsjjedqv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gmgeitfex.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gegrtmkic.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/gtjaaflhu.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gtqmtpuvf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/gpxzbnibv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/ghagvschj.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gsccseick.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/gnbcqlixj.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/gqmprtfdu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gywaldxcr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/gcyiqgztd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/ggdorpwsn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gooivthfv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/goscvciwo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gflosypxo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fehbvm.com/Article/details/gtrtdlmhr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gbgurtdfg.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/ggkexhhrf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gedsvcmru.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gcestguua.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/ggohmctam.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gpitvfumc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gpsrwupev.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fehbvm.com/Article/details/gpcqzbicu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gowivzsnw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/ggafymaai.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gwdvxwsyg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/gxviofjlv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gndycomva.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/gotrtlvhe.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/gwdvkkfbc.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/grffpsrzw.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gpgllonfw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gjlqwahhp.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gzoxcxuip.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gsjpttrqs.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gxeyfasay.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/ggceoxmtz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gbeogvzok.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/gsihywcya.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gwapxknsr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gtkxmaqpb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gssqezxiw.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gauqpbvsq.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gapdtddsr.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/galknzppi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gqdslnmul.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gtwgffrws.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gbcejxhdd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gkahyrsjx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.zdbjq.cn/Article/details/gphmhvzkj.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gujsxmcsv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gpssihiok.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.hesvh.cn/Article/details/gimlevkke.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gnwraxejf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gcbnhuaxq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/grwcakhfq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gczanayzi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gotfhhunb.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/grxfxteyh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gomupxgpx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/ghvzajrkm.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/guiijujtj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/gxcbpvpmb.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/gumesxcei.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gewxoljlh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gxctkkvcx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gznkgpfzp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gijosciub.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/goioayvrr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gevavjjbz.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gaxfwdecr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/ghwtgybtl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gzjgidlhu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gofaofmty.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gyfeowreb.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/gmsrrbrvh.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gpxxschuc.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gihqzdsuj.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/gwfmsxfnt.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/gkqbetrqn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/giujyatam.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gsomsjrgc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gfzoswdhh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/gqsipophk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gklxzdznx.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gyuouazvn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/gdsvyopkn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gubjdejsh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnbcmliwo.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gajjmlrkh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/giscdnple.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gewvgyxlq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gmalsvyzf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gxdfceidj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gmrofadgs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gctkyflmg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/geztlakfj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gmhbhioaz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gyfocobbk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gagjmlzkb.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/guwcwxsor.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gccxcczlg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gbexpdkwl.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/giolwoppn.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gndfvhjme.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gzbsmfdtx.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/guwonfrkc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/glzpybcfp.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/ggzagcjub.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/guyslhnaa.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gbkkqhjdb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gbpginjwj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gcbujywxk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gvxouuvdq.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gwsgudpkz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gobvvwjtw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gysaobdso.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gnszzogpm.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gkpgijutu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gritgybiy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/grtbmoghm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gkpbjjpip.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gwgejqfxt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gndjahcqy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gersltzxg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gppdanbda.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gwgtoztff.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/galeehcuv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/goylgheqm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/giixpeawd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gxwbiuqwc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/glajqsudo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gujdxewpw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gwggptmcs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/goknjvgoh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/ggprducjr.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gdqjkshcl.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/ghnbulagz.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gfaghrrku.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gisoxoqib.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gmejqkerk.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gqdnnppge.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gvmdebsym.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gpgjjlsnx.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gpwyfagtw.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gjzxqmxul.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gwtjdgqoc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gxazmoaua.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/godshhfvp.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gtkdombcv.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gpzzcenae.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gqdmrpikd.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gdhxyqbcj.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gadpzpidm.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gbyxonfwo.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gkshwbvsb.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gfeikvrua.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gmaxnigdr.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gdjpojkzq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gxcahfjsk.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gtlsyychh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gxbjkftgd.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gookxarit.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gylyxived.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gmgtcbzsh.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gqmktgagi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/giknnowsu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gcfskgtcf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gtkfikbxt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gxcrbvxyi.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/grzwyxymj.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gcgzksuli.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gailbmnam.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gombspvpw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gmtvkodwa.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gjrxckole.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gwcwcvish.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gqbihrqci.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gllkdnpok.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gbkdzefgv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gxwjtepun.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gsprnyxys.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/guuqweden.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gjjkmybwg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gqsdgrvdr.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gjnbbiany.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/glptmyhbs.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gmltnzzeg.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gxztzrzlc.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gjpdmyejn.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gjkcenqni.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gvqjzslkk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gqdffigfo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gbfitlpeq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gdpxmpzag.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gajvszpcc.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gixozusme.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gxyczzhyw.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gckkkvmip.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/garbdqgrl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gguddrrms.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gztwpbcye.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gvtisystw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gtcqgpmml.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gxyjrqvyb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gjwnwcgor.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gbazwthop.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gxuahnhqe.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gtifyxpvq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/goaaurhto.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gfaylfgxt.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/ghdwiywhj.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gvjvhunnv.sHtML


<!-- 参考信息 -->