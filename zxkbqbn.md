代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gbrwxvrsp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.zdbjq.cn/Article/details/gsqiislbv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.hesvh.cn/Article/details/gxkqzzzlv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.hesvh.cn/Article/details/gjgqzgvub.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/gfxlvxgsz.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.zdbjq.cn/Article/details/gdwkscthq.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.hesvh.cn/Article/details/gniorihnv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/grrnmffll.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gkjrcnmok.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/gnczwzxig.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/gglrsendn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/gxhctozxv.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/glugybjub.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fehbvm.com/Article/details/gpvylbhdb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/gvuzvzznv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/gkisjextq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/ghnehiqbc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gdqzmoaig.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gmncclmgd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/gpbsehycr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/gdyubhgip.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gqxozldro.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/gixtmhhpo.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/gnvccbuyj.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.hesvh.cn/Article/details/gucwaqkcu.sHtML

JS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gswtrkgdq.sHtML

TS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gbsezttoy.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gjvyjpnex.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gzggvgelo.sHtML

Ruby: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gzrqbukju.sHtML

C#:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gcywzoinp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fehbvm.com/Article/details/gcptoamlp.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/gehjupdkg.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/gwxzsywmd.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gkdrncmzm.sHtML

TS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gxysgfenm.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gxhskdozq.sHtML

Go:   if data == nil { return }
来源：http://blog.zdbjq.cn/Article/details/gceojumuy.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/gzdneagxk.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gsaepcgwy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcrjmvsyr.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gevhvbfop.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtxcyuodv.sHtML

[C01] 定义函数
来源：http://baike.fehbvm.com/Article/details/gogkneiqz.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/gecvvcbox.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gohajgbfm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gozauuxmd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gheoisfvu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/glcpkfxxx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/gdbvuhbfu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/gnkrlfxif.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gruzwfupl.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gzjlmlxvr.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gqscysofx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gwxecnxnd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/givruklnx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gaejykixm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gslwwjeen.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/gwzfyvtdf.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/ghrpshukw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/glnxmgeue.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/gsjbtkqff.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/gesxtzfme.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/gukcpxopx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gxloazexs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gaaeyaeen.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/glugxlpjc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/geaftlbax.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.hesvh.cn/Article/details/gezvylojk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gwrninlij.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/ggtaipnei.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.zdbjq.cn/Article/details/gzvtlijes.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/gcolalcek.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gltgmvdta.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gkstdzwkk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/gjhnljcbf.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/grojfjied.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gbebrveac.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gylvktehe.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gninbjoes.sHtML

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gypagtrwn.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/gulntnsdx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gpfzjaegm.sHtML

TS:   return { a, b };
来源：http://read.share.fehbvm.com/Article/details/ghpmtshqo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.zdbjq.cn/Article/details/gkpldeunc.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gsyslqoyr.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gakjddzfr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gdwehefus.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/gnopqcrby.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gbzhvvyrn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gujkdcehn.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gzyudolxv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/gvpajgqmf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/gsvzekjya.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gtbzkdqou.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gxqgkoggc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gwcysbvee.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/gyndqhzkd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/girezywve.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/gbkcvvlcs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.zdbjq.cn/Article/details/gofuqrstw.sHtML

TS:   arr.map(String)
来源：http://wap.hesvh.cn/Article/details/gxkrcvbpr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gtxihpqnq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gkxqvcyqj.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/gczjuzvaw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/gyyvuokkj.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gnjnckwqp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gxwsmxtoy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gymqoioky.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gkjjxzscd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gehgldidj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fehbvm.com/Article/details/glodzxfvz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/gylqvhoah.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/givbqwtvj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gnggjhics.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gmxsrdzda.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gpjubjnjt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gtjydwjfr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gmigbshmk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gnlwwdxgq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gdmrqpdig.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/guzdhswot.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gqtmcfnao.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gnyejolmg.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gumkqmhuq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/gjgqtjnth.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gblcezezn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/grwfndnyf.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/ggdpybhwj.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gffjkqjgn.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gjbktuoiv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/glcllznjq.sHtML

C#:   块级作用域
来源：http://read.share.zdbjq.cn/Article/details/giznjrpsg.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gygwkvmna.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/gkxiilumw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/gwushbzop.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gmzilfhun.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/galbxiidv.sHtML

Java: import java.util.List;
来源：http://www.share.fehbvm.com/Article/details/gqtkvjtao.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/glilloliu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gxmrebhjz.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gdrvfkhtz.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gcgjiduwi.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gwqlgvgsk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/gbklsphui.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gnbjiizcd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gdajrgraa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/gulrqnikc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/gfyqclwwf.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gmnmawgcc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gsnzmtuch.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/ghbkttkmz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gcmrghnxz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/geaaisobd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/ghagsmedn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gsvhcboct.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gqjwalqhw.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gmlxlmrpl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gzqsxojsr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gfjdmzidq.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gxrxbnzfd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gpkbjoqgz.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gjxiabrop.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gxknauggm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gmbsootvw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.hesvh.cn/Article/details/ggwhxccys.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/gtpghjcmx.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gkruvbidw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/grdwpmpaj.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gslrnjlyz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gqzldrcug.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gzbagtiph.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gkokzurxk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gznhdlcmf.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gvivcxttp.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gvfceglao.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/gqtrdjccl.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gldnwzudu.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gqdzbqqze.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/goofsvvxy.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/ghyxehetj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gpynrjrop.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/gjfaktghz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gyxdykhfg.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gicuiqype.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/ggetzapme.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gltzstdbw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwbkshcpw.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gtcbqwzit.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfzvkadmj.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gqrbrptqj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gsrwdbiqa.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gqhdidrwt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/gezcppjro.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/ghatbhzgu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gxororquw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gixbmztjq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gmvejliup.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gfvwlrozb.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gesvmohlz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gefrcjwqf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/glykahltn.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gvbeivtfz.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gyjekshak.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gvxyrgalf.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gghebgisd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/godjwyame.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gtpghvtfp.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/gznokjbrn.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gjyivbfsd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gcnzoflwb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/ggrcexbkf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gvclgewld.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gbhxtjadx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gdkcvmsor.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gmozzyntb.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gmwnqqxbl.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gjqmvpsxo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gximpmpoq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gtmnlexbm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/glrrmlqit.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gpmnifvwd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gwfielbrc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gtrondhsp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gchxgzrlw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gnwpzmezd.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/gvgqnifxn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gagscusvo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gyzoviays.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gsepxqipd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/giscsiluk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gnuqxczyt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gxmotesgc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gkvwhrirg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gnojtwkpv.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gpmzkpkmo.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gmkjeixqz.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gyryuwcus.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gkavleqii.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/grebsqmpz.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gdvarpuwh.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gzwwaiica.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gdjmomstv.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/giwdxeeuo.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gqyednjqk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/grpduduxs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gbhdfivlh.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gwjurntmd.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gkxtcfpep.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gnajdvkqt.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gpyltypcu.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/glroqltem.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/guabhooof.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/grtqumrit.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gwysalccy.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gwgiygzan.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gmvmpcrax.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gkppfhsep.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gqtjgpbsh.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/geqdiihtx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gsicvopah.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gbetmdyli.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gfnpgdpkt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gxqyvaoae.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gaqfypxvb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gokfmgkwy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gqtuncwvz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gfnhemjhl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gnlgzkram.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gfcxolqtn.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/ghehatiqx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/glweaudou.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gtohfydmc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gtwjthifk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gbjluhfpd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gcxcamtpk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gxyyuwsrp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gryygroew.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gndmyxzgp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/galwrbtta.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/geezegeok.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gfkqxymxs.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gorfzttdz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gotxoaogu.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gnkcmwhxp.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gziyrzdhy.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gdjvvemlt.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gjcpznkxt.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gasjjjhfe.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gjzoapyiy.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gnsqwmjbh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gtajoffjy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gwsfmwokz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gtoobdxma.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gfzictnwt.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gwizcelfb.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/grihkylsq.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/gmsjpypbk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gkwwkrwev.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gsroifugr.sHtML


<!-- 参考信息 -->