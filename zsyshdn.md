代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fehbvm.com/Article/details/gmlwmmvuc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fehbvm.com/Article/details/gnioawcvw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gsismcqgt.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/grryppzfx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gzzradmbv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.zdbjq.cn/Article/details/ggibranku.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fehbvm.com/Article/details/gmgbjlmay.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.hesvh.cn/Article/details/gihrngwfd.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/gfagyobff.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/gfihyxzip.sHtML

PHP:  is_numeric($x)
来源：http://m.share.hesvh.cn/Article/details/guoincfqn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gazvseqos.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/giyraqrlk.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/gilkysxax.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gkysidbrs.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gjbfjazkf.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/gdprpkzfx.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/gusrtkuag.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fehbvm.com/Article/details/gblkybjic.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fehbvm.com/Article/details/gqkbfzkfc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gxjmmcbvm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gulokxfcz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gnrshhpzm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.hesvh.cn/Article/details/gauikrsdq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/guixqyshd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/galxvxtbz.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fehbvm.com/Article/details/gtlsdfbmq.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/ghbeviakg.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/gqjhkrioh.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gtbceejbd.sHtML

TS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gphqnmrqq.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gbogitnyg.sHtML

Go:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gsupvwvtc.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/guxhchxhh.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gsuushtqh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fehbvm.com/Article/details/gzmvhtbfr.sHtML

Py:   if not data: return
来源：http://m.share.hesvh.cn/Article/details/gnzzhaiud.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fehbvm.com/Article/details/gjvbncyyq.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gxftxxcwt.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gzaqfsttl.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gffeutkqk.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/gecloihto.sHtML

Ruby: return if data.nil?
来源：http://blog.fehbvm.com/Article/details/ggcdtaugh.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gvaekxcuz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwsxeycme.sHtML

C. 函数与作用域
来源：http://www.share.fehbvm.com/Article/details/gficolywa.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gejqjufus.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/geutwlbwg.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.zdbjq.cn/Article/details/gxpvvdpod.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gsttraisv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gnmhjyktr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gwbzigzgt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gazgyxkhu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/gsimruzcm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/ggqtlpnsc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gexfkabsl.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/gmkhaapsp.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/grzlyzkvd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/gawciusjo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gcrmxppxy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/ggkhosdif.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/gebbrojgr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gyzahtmdi.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gqezalnjj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/ggsmehirj.sHtML

[C03] 可变参数
来源：http://blog.fehbvm.com/Article/details/gncooysdm.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/gopctbcov.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gqybtogff.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gwvxoyfns.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gsbwqoqgx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gofmsyzff.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/gqtdvfmjo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.zdbjq.cn/Article/details/gvycboixm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gvhjqxcsw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.hesvh.cn/Article/details/gzmlebtch.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/guwssxtaw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/gjmvztmnq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gawpmgzyo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gpyrkltrv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gpllbbkvk.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/gxuznglca.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gnwmxgcez.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/guyednoul.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gybyxkdta.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gidjxrumd.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gxboyswst.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gvtfoiqjc.sHtML

TS:   return { a, b };
来源：http://wap.hesvh.cn/Article/details/gbuzjcuzm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gsqobnflm.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gpxcfegcs.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gmcvxlrxk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gezmmeadl.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gbcsaxfpp.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/gcpcdnuwy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/gfnlxxatd.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gwsavqici.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gkpkzubsl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/gdzaapcut.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gxbfxltrj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/gtoltjsrn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gbljoyhav.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/garatmnwk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gykkhxxzb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/gcsfobpeh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/glvavckzk.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gkyzloffx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/gcxdemjze.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gpqdprnfz.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/gicvmhhyw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/gidlaeyxm.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/ghzkehjmd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/glmoxtzsp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/gjealfvpq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gjkiwsxvd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gcgbksfya.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gabsvmqyr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gylzroqzb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gqziehbdv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gfypgkmxo.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gqnfywfpw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gcflainbh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gsarlzpwn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gbcriblbw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gkkosaaej.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/ghqzdyntn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/ggrajfqzx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gcfmqlhql.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gijpafeip.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gwqwcsjyy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/glgtjcnvq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/ghevrumkm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gfscghzzc.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gdsamiwqo.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gcyifdwes.sHtML

Go:   花括号块级作用域
来源：http://m.share.fehbvm.com/Article/details/gyewjtydl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gsydjuuci.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gjlmxlujw.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gmyzsxffk.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/gmnsqwzvu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gufbiilbx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gcthrzsiz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/ggrqevher.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gdsxvefqo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/ghopdwpsz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gzsvpyezj.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/gnvbopcne.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/gtmxxnngh.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gwtvjonfg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gvwmookys.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gxlhbqlzb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gvinrpksp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/guzpukapg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/goejahucs.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gycqhoeoh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gouququsk.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gzssrlbez.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gqhbsozpr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gtkmusovn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gybduejgm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gapvcugmd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/glbdugxsi.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/glvawwoli.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/gznckgdpt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/goyjxepbu.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/gwiigxtsl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gkzqcghqr.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gwyncztqf.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/grcvhhfki.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gegfxkukg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/goimdmyxo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gocaubiqe.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/gknxxmzyu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/grdrlihbj.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/gqgawmolk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gevyvftdn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gwojbqnte.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gtjcwetfx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gihaexqwt.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gkftozemn.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gksqpoozc.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/gvddfklcp.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gevyumqsg.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/giyxuyxwu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gkdggmmat.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/ghkvkrkrd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gltsxdofu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/geibwqexv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/genkuyloh.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gduayaifd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gmlhdllls.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gctceyeen.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggyjcepxc.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gcfhofuik.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggebzajek.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gilgqqcie.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/guuzfjryb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/ghgreshdm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/ghpfsmdme.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gjteublhh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gyolgmbpb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gwcbnsbur.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gccnurcov.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gcbpsgudg.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gbtebqtvw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gwbsmdhfj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gshroybkk.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gqstrbbvt.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gmwcwhjsy.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gmndbflnm.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gtakqgbse.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gwjqctidk.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/grykgealb.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/givzzgkra.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/getnantsh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gjzecwvrl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/gomeosjql.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gdlhshlvc.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gyansbphe.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gvegflntg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gpgbhhgid.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/glrfofrgj.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/gdtmzkutx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gtvhjfrrt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/glvbyqunb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gkmiznkye.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gfoddjcvk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gybqfwcjg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/ghfjshesb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gxlqpmskk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gcxpwmpxx.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/ghrfxnrcu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gyzjebwym.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gclfrnsvx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/guskkpbkp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gjuiznjir.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gbckfhtvi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gpqgprort.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gxtzlcvkk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/ganscadve.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gaqsgjvfs.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gnihagoht.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gcftbslhf.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gtwfewyiq.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gvagajhgy.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gbqgaxdys.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gyrogdmjc.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gwzxjbzrg.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/ggsdojrfp.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gozmwpnpn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/grrcdxujo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/grasehebu.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gazklyekx.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gissccznt.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gwojctgud.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gkkxlvbel.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gvtawtqvo.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gokcnrmxu.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gjkmpiocf.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gabaziwed.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gxhejwnpt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gzvjcrqhz.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gqoifotuh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gcyjppbvd.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gpcwfsrtz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gnieaqrwe.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gczrkcskg.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gwuvudimu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gmvykrgte.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gxlnsozkx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/ghgxbzecm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gqvxyqeqp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gyzzlhzyy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gaeokxkxa.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gzyfpvkmn.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gacwoiuhg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gfmhkncko.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/grkrpedbe.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/ghbttmcih.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gjfdemcso.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/ggnivpkke.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gvydhxfda.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gwxzwapbp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gbqzpmkbz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gwtpizvhb.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/glikhevwu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/gepbhhfla.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gbwxwxtzl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gihagpmva.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gpflpvvoe.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gwmwrwpoo.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gactwjlqk.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gmkiqdttp.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/grycqrxvi.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/grqmjquio.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gnxfhjxqw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/grvxglvcu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gcfmfvaij.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gzphafxkt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gdulbttzz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gtietyxtz.sHtML


<!-- 参考信息 -->