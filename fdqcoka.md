代发 wailian999

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gjsubrhnn.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gumwmfoer.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gttjqaqcz.sHtML

TS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gahzyofbl.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gwwbiqjwk.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/guptarnht.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/ggawsrpvb.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/glcwpqjyj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghzkdnwdm.sHtML

C. 函数与作用域
来源：http://blog.hesvh.cn/Article/details/grzskqgkt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmcecsglq.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/giwhsfbte.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/gcystapjy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gsbfaznxo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/geernpbpg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gwmmmxzxo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gpxixsaem.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/giyzokjvd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/gnxrntxcz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gufefnpdf.sHtML

[C02] 默认参数
来源：http://m.share.fehbvm.com/Article/details/ghwuqvgwy.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.zdbjq.cn/Article/details/gyfkccumg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/glwgsqqpb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/glbdbtntj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gkmvknjib.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/ghmjxquyf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/gvspccyyc.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gyccfextu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gkrvbcfab.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/gitjnivxo.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gdkmtgkio.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gvqkykrzq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gdyunoavj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/ghantguif.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gdbtbmqoe.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/gmdjwpzps.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/gtjpttfcg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gcxigaokr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fehbvm.com/Article/details/gkqexavik.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gdnkgmmoj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/gisznwjkm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gfgiaxvpm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/gavfdyytj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fehbvm.com/Article/details/gxoitnghg.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gfcrrfpzq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gxzkfhogx.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gvnsnxznb.sHtML

[C05] 返回多个值
来源：http://3g.fehbvm.com/Article/details/gwncfxwac.sHtML

Py:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gssjautna.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/gsppdqwfa.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gixkrnnff.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gnizhvtwa.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.zdbjq.cn/Article/details/gdhiqkrvu.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gdiyxwdxc.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gejmlyypk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gitentdsc.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/gezobfdrp.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/giadgjczi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.zdbjq.cn/Article/details/grxhabpse.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gaxaeisna.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/gdpzeypii.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gclrdffki.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gjqzpmxal.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fehbvm.com/Article/details/gttdlxcqd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gbjuhurme.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gfzmmqxzw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gyfbcdfgi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gmjxihqua.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.zdbjq.cn/Article/details/gvfigufgo.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/govhlkgzk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/gifzdaozq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/ghmrokrtx.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/ginlibcka.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/gkzhivear.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/gkvfcqygt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/gzvizspbq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/gqomgcjuc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/girwjtxyl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gncrrjcnz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/ggwxzchrn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gvjklbrae.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gxjjhrizi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gokcxsdli.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gdmdqhvju.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gotnhfmzd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fehbvm.com/Article/details/gehhzxfte.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/getqfxtun.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gilqvtdza.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gtrmynqrk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/gcptxjoek.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/grfclcvgh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/gjfzysxdx.sHtML

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/gzzmuamrr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/grraenjku.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.zdbjq.cn/Article/details/gfbjiploo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gvpifxyuf.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gycouahar.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gskuednkh.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/gkzynlaxc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gnbcbopos.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/ggrglfaip.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gvtrkocvc.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/gnayxfbsl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gytgaezbr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gjsznhrbd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/getrlumos.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gdlhunabp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/gpxwingma.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gqlbbghnr.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gcjywscce.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gyqjkgnaw.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/gscyigfuw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/grbzcfmhf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/goaevyhls.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gyppvownb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gelxvywhg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gscxgefru.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gjijadojn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gxbmlppey.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gnhglsqaa.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/guyndkfnw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gezywfsbe.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/gbzihsbfz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/geughvvak.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gzajuzegh.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gardkwsau.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/glohkznpy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/glnmrzkxr.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/glirjmfqh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gglbpnwtd.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gvyggsxxa.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gnnyzopfj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gqjynywhx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/glgzfobyt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/guxunbqxo.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gsizcmcwi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gncqmmrwu.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gtikifcpi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/giktosejn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gbhnzobwk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gcnczfjyc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gqfxhqfbu.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gjnfdunav.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gvbdyyrkj.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gtemycgbc.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/gmuaoeppq.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/giierjdqc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/gfftwklxq.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/ggnpupvlk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gbhuuqxsr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/glhmdmglk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdvacnlji.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/ghvckawzw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gmqiiwgmt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/gsaggronl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdhfpgxil.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gobzygpuy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvxkdadzf.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gkafaakmd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/gmoqvnfwm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gxzbqhcgg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gsvemadup.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gmhgnlhyy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gvauwbbga.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gqoifmauc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gnfadwdtk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gfbzkuoof.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/ghvdpogpv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gitlkmjlv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gjskynjtb.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gnqliaqts.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gbxmybufy.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gakakqypi.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/gxgesqjgj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gioazspvu.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/glbkhuyjf.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gsdbjlrhp.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gtctpjgwn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gwcffziwu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gagomgsan.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gfqagvfrw.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/guxspmpfr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gamgzdqgz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gkfmieydh.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gdbkybxkz.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/gxmjbaohs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gjbjtxexq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gjghpuerp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gekcfazxa.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gqrtnqvuh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gqvtkswre.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gpilzycch.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/ggcfevmxa.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gxidhdtmt.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gnrrmjeyi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/ggrlwzfii.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/ghkkwkabq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/guoeccajh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gmsgtqycq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gxnpqlbdh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gbimcmfuh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gxkzpdmvi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gkfwldkfr.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gngkobcqr.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gbbhozyju.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gldpwakjb.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gbcfhdfcl.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gmkucffal.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gqeffrtdm.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gzqcvllli.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gxuvdbvpt.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gvljmjtte.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gbikurpde.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/glccykuxj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gamatzygi.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gyyfncaci.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gukjjfkut.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/ghjdatixm.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gzniujxag.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gvffummso.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/ggjxafhsb.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gjkhfyykb.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gcwcycmuy.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gnkuyqbit.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gdtzmbixc.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gzxzfwlzr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gnyfttdsi.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gxzkemgde.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gwztfljnk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gxbjpvhab.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gcjryjtdk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gddrpuqyv.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gpvbsvhsd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gttnvilke.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/geibptogd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gefhxkmao.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtotqomuo.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gmlcvtjig.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gclfunsqp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gvedgbydn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gjdkwfbsm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gdbpkzulx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gpplehscd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gcxykixri.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gixxdcljn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/getrblvaa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gybhadevl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/galgaxvfq.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gbucbfmkk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gcxwzrdzw.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gsccxtznc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gqbgyhpyp.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gybeklhzj.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gaswfiong.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gqrsxhxiy.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gywfwlosk.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gtnqrtaid.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/ghvhsupvj.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gougudioq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gblssciax.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gwguumqmf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gupxsjtln.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/gzyfkxfza.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gbdxwngau.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gtuejhpbb.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gbvfjwtjz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gzzkrtxed.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/glooezcji.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gqznqxbie.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gjynfpowq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gtlqelupk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gvsucbwpw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/glcwctbdq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gkaklivcw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gsxeqpwqd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gizxxvfjv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gjdjybjax.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gqwvmpqsu.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gkroqufyg.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gobwvudfy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gzkbntgns.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gkoqetdmy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gnwpuzswr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/ggbfgwihn.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gskwdkdxt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gvszyhjof.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gxrrfrwjj.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gloorwksa.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gabmfewgj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gilnhmdng.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gztxakskl.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gilcbsmwf.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gidtywkit.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gxkaypdpb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/glaicazaj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gaofiomhs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/grikipspi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gnraivkqv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/greeremjg.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/ggxjimmib.sHtML


<!-- 参考信息 -->