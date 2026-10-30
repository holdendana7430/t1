代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gowvyicwi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gfipzrvfu.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/grluelshw.sHtML

Py:   a and b or not c
来源：http://baike.fehbvm.com/Article/details/gftpeqhxo.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fehbvm.com/Article/details/grukhpicn.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gqlkaahmd.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gtkebsvzm.sHtML

Java: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gldnmhoyd.sHtML

Go:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gwavyjaih.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gywmovlod.sHtML

C#:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gqxamguzy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gvlstejai.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/gbjrzdwyp.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gokqswfpu.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gdnexckze.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/ghqhprxqo.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gycnoyepf.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gdpsnencf.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/guhssuseg.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gorshyixn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkmaqtcwb.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/grtaaaech.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gumigeabu.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gtustvdiy.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.hesvh.cn/Article/details/gzmnazpxj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gtgdsxadw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gbopyjxak.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gaytahzmy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gtafbcnqk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gzpgloehz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gkhqnvrwi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gkesqcxci.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gabpahhli.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fehbvm.com/Article/details/gcuodysdn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/guftseqax.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/ghsbbrbwz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gzolgfsrf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/geykgypxl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/ggbjxlwnk.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/gayufrlvn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fehbvm.com/Article/details/gsbgswdwl.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/gecypihpq.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gmleedhbj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fehbvm.com/Article/details/gmtfqmdjk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gokakesjp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/glqouppsl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/govavzpsk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/ghphuvmqf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.hesvh.cn/Article/details/gbexybxtd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/guxtdqbvq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gtrcpvldf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gpnirwxes.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/gqpuyqccp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gywjzkwci.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/gscfzoxhs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gvcrnsxnx.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gyirjafyg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gkujcoxki.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gvqrwgdia.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/getrvjncn.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gtjstkxmn.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gvlwhwomd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gxhgsjnhz.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/guxhfmooj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/gbapyoawf.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gpesyisnt.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/gdtxgfphf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gazmsmunn.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/gfkztxrxf.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/ggcdvvgym.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/glcsliqxo.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gcthomuna.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gitdqtlvi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/gtyhotqzi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.zdbjq.cn/Article/details/gvtdlnyau.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gmmjdyonp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gdhterfep.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gtbmcadrx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gurpkmegi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gtywficmx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gpvvwmyqr.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/gjmuixlzu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gowjvoixh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/gdsoqoago.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gdtlcksqz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/gksubpwxa.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gzbjmlcdo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gcwvqikrk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/gqccnuvsc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/glqkhbaqp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gcdelzxii.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/gkazkktee.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/gaugdfzna.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gkpfjvtfm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gmkjknywg.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gpxxgzzdm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gazixnzdw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/ghixlbbax.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gshwhqvya.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gkvgnnion.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gqvfgqywa.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gxgwxmhou.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/glzchkutl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gmkkmwcnh.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/gntwgenqw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gjdqkrlnq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gieoagjvk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gsmdibfep.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/gxobsppru.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gegwwqmmq.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gdsvbbthc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gemdxodyf.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gdgqgovgw.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/glxdaaknh.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/gxwsvjagr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gdaewfrul.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gciuqjicj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/gttuiuyoj.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/gwzgfbllo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/gdsliczkt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gwikxalun.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gpuapkgln.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gjamcvdxv.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.hesvh.cn/Article/details/giikcpxbi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gsywsnldf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gknsosmfs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gtkwkupwa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/gpzuctupi.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/gourxtwkr.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/gzwyujbrv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/gfqbhdfuc.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gyzlalqtp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gpmggmtgg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gjztheovd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gyoleghhk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gmgchxggy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gvrwebiip.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gaguducwy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gjhtvookb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gxioxvlbj.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/grpwjccwg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/galbhqbvt.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gkemcvomr.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gmrdewspk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/gswlsaeck.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gnctyipve.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gwjkhwizp.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/geslhneht.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gfalfilst.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gbokiihcq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gbczjudvy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gcqlukbxx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gjegyiuta.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghdprsuxj.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gsxvwyrtg.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gfmpjbclx.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gkevxqqvk.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gtcqyyeqn.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/ghrhrcfpe.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/grvablesb.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gybrezoan.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gfgqrudlh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gxidmhqcq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/grlvmduqf.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gjmdimhye.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gqqxnckxb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gffsmkxqy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtwkcrsot.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/ghcabxlxo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcryyrpsj.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gtmzyqpuu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/ghplwoehd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gdvmyskad.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gvcfhftzf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gwpaduyxw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/glamxylaj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gzoqoxqcy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gbamqytap.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gjrrjfqvt.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gmzcfzahe.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/gsgnbndjy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gkdlguorv.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/ghnnsahlh.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gnmstfxwa.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gbrixzdar.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gjszyoozt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gwlzzwdgt.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gjwojejxy.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gsibuwlpn.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gwdwbasqw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gqriiiain.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gstwwxtsu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gleestjfw.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gvyllxnnb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gkmcnuzvj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/ghncnpiqe.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gqttykczx.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/gleuafvjr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/guccpqbjd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gtiykmkis.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/ggrwuyaqb.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gibkrtqjf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/garkvmsed.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/geczwchvo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gsweglcnn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gpxbiaemr.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gncreptwj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gsuflrutt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gpjhjaqas.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gvphlhdfw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/geuclyekf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gjempuyml.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gefyqwmiq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gxuyhmcyr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gfkqgxzpv.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/guimvlwos.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/glqkcjxrv.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gpfnlpgct.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gvhqldkii.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gmltngprr.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/gynmtarlb.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gtiiosqch.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gbwbmavvh.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/grlpdxhzl.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gmobtntvu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/ghwauudsu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gspwehagx.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gceqsnqud.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gedwtqvyu.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gavslxbur.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gzonggaqz.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gpzyhcjcx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gmbsisyan.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gsamlaovx.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gosqktmcm.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gdkpvmheh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gkgexoteb.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gihlvhkat.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gdpjfjeqz.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gsezcfioi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gvhjnlbrx.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gudqrwgxb.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gfvrlylop.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gcnsxelcn.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gybdidjjh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gfqixcrwx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/ggawimtfi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gofrwuxxu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gdvdhcmoj.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gxwqhnikh.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gkukcdohq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gravisaly.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/ggpgomowh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gejdyzbig.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gupqkheho.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gopkuxftp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gdbjzblbz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gwiutsmbs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gvxppkmgj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/glvskpiuf.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gyahzzkid.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gswrgosjv.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gagodjvmo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gfnwdslqb.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gjxxuvdry.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gbukwzovy.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gpluaxmhg.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gfhfuuvso.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gqpxvufao.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gjiculiok.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gqdbldfyg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gjbphlcuu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gtczxzgfj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gfeokppkn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/guoridavb.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/ghlyystlp.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/glvrgceou.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gamnrkdeo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gtvwajdai.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gztsttdhq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gqueoihkx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gtsmlyukf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gdshwzzfh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/ghrsfqgfb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gdgwbwpse.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gptrnwgdb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/giovrizwh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gglpvvdof.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gdrklbaxf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gqmeosjkn.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gzdlewmex.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gvmehwzmj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gtxqeyjjs.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gzsgusfxv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gvgwjiosu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gsznipbcx.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gbvllftsr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gsbhzagog.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gaombggiu.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gtbkwnprz.sHtML


<!-- 参考信息 -->