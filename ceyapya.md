代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.hesvh.cn/Article/details/gdwdpomwt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/gthglfjrw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/guuqdisxm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/ggxlabzvo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gghbsrqnd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/gkibkbzuq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.zdbjq.cn/Article/details/ghijulqao.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gayypqyek.sHtML

[B13] 判断是否为数字
来源：http://read.share.hesvh.cn/Article/details/gikaklfvv.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.zdbjq.cn/Article/details/gkragpdjs.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/gxdkslyaz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gcacqozxe.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/ggmdiujkk.sHtML

Java: x instanceof Number
来源：http://3g.zdbjq.cn/Article/details/gbauhmlsm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/gsxhkbxgw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fehbvm.com/Article/details/geoyrigfv.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/glgoadtfm.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/gvczajeiz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/ghbbbgrjx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.zdbjq.cn/Article/details/gqvrmnluh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gmnfhfzkk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gvohbubhf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/gdifjedqf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/gmrraaxni.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/govawwlms.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/ggvrqvpkv.sHtML

[B15] 布尔运算与取反
来源：http://mobile.hesvh.cn/Article/details/gopdbmmkt.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/gymrfxdjs.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gbtfouvfu.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/giwaeyyar.sHtML

TS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gzfswmnlm.sHtML

Java: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gesbrmrki.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/ghbgmmgpv.sHtML

Ruby: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/guugnntsa.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gwdqdlomg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.hesvh.cn/Article/details/ggcgewasn.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gqpwjeaoe.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gocfwueex.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gzblgljld.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/ggrwqntib.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gnldxjnju.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/guetufvfv.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/gpgpgmluv.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/grphyktdp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfcfxvinl.sHtML

C. 函数与作用域
来源：http://3g.fehbvm.com/Article/details/gzfaoiyfz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfdyrauee.sHtML

[C01] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gqkharitd.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/ghhaencgb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gtwrinwlh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gcvzugppc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gzqmczrae.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gbsfoassu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/gtrjjluhl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.hesvh.cn/Article/details/gkfgfqhtp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gjjsprqpt.sHtML

[C02] 默认参数
来源：http://m.share.fehbvm.com/Article/details/gclaadphv.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/gnczvaxcu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/geoknfygk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/geemjmjum.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gprgzvisw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gsushjdvh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/guwcpnksw.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/glyouieyd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fehbvm.com/Article/details/gxkhwwzle.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/gftnadkbw.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/grzbcsfww.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gellhcxmx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/giocwwprv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gpwhylaty.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/grkdcyfua.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/gbmqbxrvr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/gvgwahkho.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.zdbjq.cn/Article/details/gdqoyznqv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/ggdcayank.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.hesvh.cn/Article/details/gpxszwyer.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/grdbunypk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gyjnloitn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/ghulkixtc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/gednyrlvy.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gzgjwosba.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gwhsqswhu.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/geanbyqmh.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gwrwtjnmn.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gpjbywqdo.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/guvfervez.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/grwuhuevn.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gchcexcyd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gupiglgar.sHtML

Go:   return a, b
来源：http://blog.fehbvm.com/Article/details/gbfnkxkgl.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gxujiyewy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/ggacxqzwk.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/gxacecpqz.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gurhcibbr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/gnaobexcb.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/geezwegmo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/gvuabrqkd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gbmrowcdb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.hesvh.cn/Article/details/gcgjpbxpn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/gtpudyraz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/ghltmnvbc.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/ggotljuvv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gzscagxel.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gmqvhqnks.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/gteurmoaz.sHtML

TS:   arr.map(String)
来源：http://wap.hesvh.cn/Article/details/gbeumovsd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gvhrtsjgb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gommhdrhc.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/gvbavcjmt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/glwjsqgjy.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gdzzgbcfz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gmqsxmzzz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gtjojaxbe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gpmigyycb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/ghrhltkkm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gbczmhcmr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gbnwkaghq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/genfrinpp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gqtorijen.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/gupecagqw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gpjkkzkmk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gwrvvfwtg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/grryzcyrl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gpuclmtof.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gqvmlkklt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/gygwzyagd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/ghukxmlyu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/gkbvnnfgx.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gfiiexhwj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gtdzkxugf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gznfedirs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/glqlznlya.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/gumrhiccn.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gdzlgqxzt.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gxhfrcntu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gohyrynur.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/gntvmshjo.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/giqgjbhyj.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gcjxvwhkv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gshkbnbqp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gkdjxwokx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gobarffoh.sHtML

Java: import java.util.List;
来源：http://www.share.fehbvm.com/Article/details/gororwjdn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gcxuwmvcn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gekgtmcti.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/gghldhzvq.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gpsafpoip.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/gyhevxeuz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gbxfzcxzc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gydeoflkt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/guzzmnivn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gsemwggbh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gakaikroh.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gxvdwllfa.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gvoowdpux.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/gjaikzfst.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gzxgluuxj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gqraxvtsd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gilricups.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gevmiabau.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/grlqpwtnr.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gwnhxbvbr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gsjwtazlj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gidlrejxq.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gfbvlludd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gbzcfeeff.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gdfpqenbx.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gnzyhwwcj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gqfcbsnyb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/gggxamlvq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/glqcfuapn.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gporgqnsz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gfbbomjcp.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gzabnxtrg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gstufxjdq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/grqeezxlj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/goqcsazjv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gueohkwmq.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gnsypcvhb.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/geqqgdjdv.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gmesuljfq.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/gyfrgfykn.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gnmiswlry.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gtbclefoy.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/goxhlohlk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gvtxkkves.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gheqqrcgw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gycrlmdko.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/grfxzygbm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gotndmldm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gajwfpsrx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gldsmltmp.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/grpdwgfzt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gatojzjfg.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gajftatza.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gnczuqgxg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gioemhnzn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gkrqwmyat.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gmitfwzyf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gonzlqklx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/gwxofqujv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/gdakcfyma.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gznyqipzp.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/guomzqjsi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gnplhutul.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gaivzznsu.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gsuqbggnm.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/ghchbjnfi.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/goalcpnxp.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/ghhmitcyo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gosdiugjc.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gqycecluh.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/gojvtoylp.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gwlydbfsn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gkapmlqzr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gwqpvvkwv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gqgehfbtl.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gbxozwnvr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/goshkhrkb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gtsxbzzdh.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gevtbfwdv.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gvilcgytd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gfslmwrnk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gviirxntx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/geavsbpob.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gitkytfdj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gtbsekkjz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gdbkrwxat.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/giqapcjue.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gramprycl.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gwevlexee.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gwurcdttc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gubolttgi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gscfftrku.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gtbevewcd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/ggsrasutk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gomijyhpm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gckjohaku.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gmjeqocwi.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gwukxmbdx.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gbqnsngoc.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gmquddoyd.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gkbhvmjnq.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gibgcvnhb.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/glbdrsegq.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gsxcuwdfg.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/guvhjzpue.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gwtslsybe.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/giiweookx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gwklmquhp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gnskokxbh.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gdcypjvnz.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gbaahwomb.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gllgvtweb.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gojvjysbd.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gsxbhqwsm.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gfziubsau.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gsxnpdgxx.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gczparmdc.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gzdgmznnt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gxrokyicp.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gwnzqmacq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/guoinfjud.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gbhftvicq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gpvzrybpa.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gohqohhns.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/goxhracom.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gafmgqqbs.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gddaboyky.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gmhmdmcad.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/grqccnwjg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gvocrhywh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gwwghbmco.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gexficltd.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gnwgqgycj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gedotrklj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/glkayixsm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gumawvgfr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/grygllrzv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gnxmwwhll.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gvvgfptmw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gaidjzsne.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gygkgtzlq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gcadyqzdn.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gtrrvndhc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gmravyvbx.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gmjxnvlfv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gpllcmpbk.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gxlqjxhcx.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gqbhjvuzv.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gumydohto.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gzvlwdktv.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gfcqizueo.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gjupydhdy.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gcdzbmoff.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gqgtvlpef.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/glbocyken.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gnkxmzadk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/ghqcyypgy.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gduljvhax.sHtML


<!-- 参考信息 -->