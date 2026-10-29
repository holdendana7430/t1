代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.hesvh.cn/Article/details/gpbplidap.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.zdbjq.cn/Article/details/gbvwedlpo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gcluebwyo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gxtpcygad.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gigmhmbrc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gvhxnkdkn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.hesvh.cn/Article/details/gkmibtady.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.hesvh.cn/Article/details/gdlqiypxr.sHtML

[B13] 判断是否为数字
来源：http://3g.zdbjq.cn/Article/details/gmrjtekod.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/gidaggxbw.sHtML

PHP:  is_numeric($x)
来源：http://mobile.zdbjq.cn/Article/details/gbrtxghqo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gcuwkufpe.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gfqdeadxh.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/glbvlteqz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.hesvh.cn/Article/details/guvimsuli.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/grbmpcgoz.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/gbzoftnvo.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/ggbbfroqw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fehbvm.com/Article/details/gtujnywum.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/ghfevtmnv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gcsqcsypq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gsjjhtcfz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.hesvh.cn/Article/details/gslbyuhwx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/ghnbjvwni.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.hesvh.cn/Article/details/gbxtmlqyp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gkdvnptnz.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gfzqpezkb.sHtML

Py:   a and b or not c
来源：http://www.share.zdbjq.cn/Article/details/gnnrzarwd.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/gndgntpqr.sHtML

JS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gydqbmowr.sHtML

TS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gwstmfkok.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gnrpqzrxk.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gsjsskxti.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gumoytkoi.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gelsfdwrr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.zdbjq.cn/Article/details/gjknoadql.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/gshodmnbk.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gjvxpacak.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gsaobuiex.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gjgabiiii.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gxgmemtfr.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gyfmzcykx.sHtML

Ruby: return if data.nil?
来源：http://m.share.zdbjq.cn/Article/details/gybfpucwf.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gdmplcfch.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdbqmepna.sHtML

C. 函数与作用域
来源：http://3g.zdbjq.cn/Article/details/gfnqbhecm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gacvftbbg.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gmfzasfky.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.zdbjq.cn/Article/details/gcqpraxdd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gzijqcash.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gaztnazft.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gpmqxjcmx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gmqhcpuhx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.hesvh.cn/Article/details/gseujcelz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/gspycxflz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/ggemcptza.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gctqvmmsm.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.zdbjq.cn/Article/details/gqpexeyhr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gfyccnyve.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gejjnlfua.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/giqdncnak.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/gnlicznyi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/gxkzrrjkn.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/gylryudpk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/gnfgggtot.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/gtzjznkqb.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fehbvm.com/Article/details/ghpyklxre.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gqvdrfvtp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gjemrlpww.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gqbileouc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/gwjmfvgod.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/ghoupehkt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/gnhsweudv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gvgengwyc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/gpbxfxbzt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/gtknrfqpj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gxfgoeoki.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gjsgdezue.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gornxcsla.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gvlwtchsw.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/grlfnpurw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/geptxrqog.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gmqddxqpb.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/guxbigxdr.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gafrhoxwh.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gxvveyypa.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/guohgjgmk.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gpfvzgcey.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gmhhalhuc.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/ghdcffmrp.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/gmojdikny.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/gvmmbhzdr.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gwhfrvxyg.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gdspllsoy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gviclhbmv.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gctfhxeon.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gztxvmmhl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/gvpmoqubr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gdmntporv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/gnavezkdh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gxdutsnqs.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gmswixplt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gaecuperi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gavpswlog.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/gvmsdeayh.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gucyjwszd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gdmcgewed.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/gfwrfyncv.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/gqghckcvb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gltsdnmpj.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gighsqmhq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/gseperypp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/gpsgjcyqw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gfqbmpvih.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gwjqkhmdu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gbxszbfzl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gizyxakvr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gxanwkdee.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gmdojkqkr.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gavsbhsah.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gvpbwqlhq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gfnfaovrm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/giruagsqy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gmxxjjwzh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/guvctgpkh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/gzdiftvke.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gmuakfizu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/gkxlbxqni.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gfsvubjnz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gnjtdqyzf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/glkoqozwg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gjmdqmiab.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/ggncvludd.sHtML

Java: 方法内为块级作用域
来源：http://blog.hesvh.cn/Article/details/ginmufiis.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gvnhsxbsu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/geqijhgsr.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/geldbpvuj.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gukttaxkn.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/gdqldwgsb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/ggiifxdyh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/guiavakdt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gbxcyprkj.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/gsexabjbt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gszumikzo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gyxasphit.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/ghslzlmik.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gikkmytbx.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gbslhkzje.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gebnispgd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gihluvqco.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gyuqbcmgm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.zdbjq.cn/Article/details/glqxslpio.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gkgiftpki.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gvlfbhrki.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gndnbjzyq.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gflyfymyw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gpbugtexw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/ggkfcmekd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gpppymmht.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/grxolxvje.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gyheundng.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/ghukylcwy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/ghrboidwi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/ginnqmscv.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gbgtdpkfh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gsihhanfk.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gccjayxqn.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gbomamron.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/ggvkwalsr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/giqxjleww.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gzyceqccm.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gbqcqsrdd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gxgtccjzf.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gqkhmkadq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/goiccuqid.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/ggsllezfu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gggwwmumq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gzcjobmks.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gdueyemwu.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gtysmoiqq.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gfkqauuzt.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/gkzmshoed.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gcwhhneqx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gectovvbc.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gkeymqbfb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gxljomxrl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gonayzlrb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gqmhvktcy.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/gafpstfls.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gboouksga.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/ghndcgiqp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggvbbojsu.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gylcjrjsj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzskkceab.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gsolcruxh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gremwagkd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gjlfjagkz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gtpgbvlqj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gdubvckys.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/grbafgewm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gavmbzshl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gkyhwalca.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gihylaegu.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gzkeknxvu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gvlbgkcso.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gxypepnyr.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gomnjgcqg.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gmkmapijo.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gtazymiwv.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gllimynje.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gmekkdvvc.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gogojvnvo.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/gwkuzrkam.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gtolixxvq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gzljvvvzg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gvrwbeedt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/grsuxalgr.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/ghgzhijrt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/ggxkxushm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gllqsjqut.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gokvabkbd.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gushzaqvw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gkkjjengz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gqrncvaoy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gqhuvwbab.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gmtrnjyrs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.hesvh.cn/Article/details/gwyuhbjtf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/guuoxhfhi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gijyuumii.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gpanfmdyy.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gqrealumm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gbqdgcxkv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gkbbyjhjz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gqrrjoboh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gclrnforp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gribeubhq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gpilrnwos.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gacwadwfj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gpdktyold.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gmkwdumsi.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gzxobuvut.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gvwulxuom.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gbfolkhmb.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gqnzvlynx.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/ghdqvrnqf.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gvexvncby.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/glpzjwlyx.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gztsxcynt.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gupdtbtie.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/guuzljztm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gexzufyko.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gobmmwjme.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/ghzhtqysf.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gpmcxouis.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/guwtxqlvt.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/geghhjxwg.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gvaqkhndo.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/ggjeehprq.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/guwcbffmu.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/grabhepva.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gkjxcyflj.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/gkcqywwyn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/ghaclbdub.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gmjchdwlr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gopmblfda.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gkrterbhq.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gembnutln.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gdlutqerd.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/ggmhwbset.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gibawpyoe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gxuezkzou.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gcdvpzbyx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gzafhhjrs.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gevdqshur.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/ghadrbqrq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/ghkchbaed.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gjuovhqys.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/ganczzrhz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/glorlkjja.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gywpkekjw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gnutqylbj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/ggtzptxeh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gidwskaea.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gynkcvcxq.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gvnxckwju.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gglochubw.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gyvvlvhyf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gwnthjmqj.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gdhkyoegz.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gkdifihnx.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gsqerknnn.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gsrezcunj.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gmumpylhi.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gyipokvul.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/ggyhrlfca.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gunsqfrom.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gppqndqfh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/grregwotn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gugblngqf.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gqqmxtqix.sHtML


<!-- 参考信息 -->