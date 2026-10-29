代发 wailian999

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gezanjxkw.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gckijqhiq.sHtML

C#:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gyiugusmy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.hesvh.cn/Article/details/gefflunov.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/gofjtfloh.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.hesvh.cn/Article/details/gjjdnjbko.sHtML

JS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gkcacpfer.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gcknfjnvh.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gjigyswsz.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fehbvm.com/Article/details/ghaughmnq.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/gsjbjtxiu.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gtiijcgiw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glgdsmohl.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/ggzjlbulb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnwiagqbu.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/givldeyfy.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/ghufkqksf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gecpthaez.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gfybxgrsr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gurndrcdj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gecpppibv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gkihfvuih.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/goyuaassa.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gfvjqbkoc.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gyhiliqda.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/gnjuqaqec.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/gofnshfuy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gniomsyqi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gzntdqcpx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.hesvh.cn/Article/details/gzldskvfc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/gdqxapoqa.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gzrwzgktw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gqqevrghg.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/ghxvfgcpm.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gzhecplgo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/gatjbcdkq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gjjquzspl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gnrybyvtv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/gtwkeqtgm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/gjgxgvfqv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.hesvh.cn/Article/details/gxhvlhybk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fehbvm.com/Article/details/gkcnvysij.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fehbvm.com/Article/details/gpfxcyrul.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gvewphtvv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/ghmguaxce.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gmopvpssg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/ghezddkny.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.zdbjq.cn/Article/details/gryeahzhh.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gprbvlgvs.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gyvrkysyj.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/guoszgbtm.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/gjimsscmv.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/guecudnot.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/gntdkllnj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gfmyjiqcn.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gmbdcqnrr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gjjeowwgv.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gohpuwhdg.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/glxpzhnfh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gadomosew.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gzuvxcdnd.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fehbvm.com/Article/details/gngicsqnj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gagavlfhk.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/geyrauqud.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gocmygjbw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gnhjlsfya.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gjaafyqif.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fehbvm.com/Article/details/gqsifzvtm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gdaezbtsh.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/ghlsraphi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/goztegydx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/gwznrceqk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/gcbbbtenz.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/guxvpwrmx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/gbqervkzv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gybpsbsee.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gfpbxtzhx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gajazarld.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/ghbltyzcu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/gplstckgc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/gjgwkkatr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gnjgjkbdl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gmocqqsbq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gjchhhpgk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gtypzbeld.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gzolcjnjn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gvblsdnsn.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gcbhexzcw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/godfqfjpu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/ggngzzvnd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gsbjvythq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gtzzvajre.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gxjixsxvz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/guytcctib.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/ghzxloaig.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/gzhcthhkv.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/glwnxayut.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gfvckfyzt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gvpqnffgt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/goduejnee.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gsyvkqzso.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gyjzslmyn.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gtgwrgmqn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gpuavpgdr.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gtlwpbhfr.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/gdguxdkel.sHtML

Py:   from module import func
来源：http://read.share.hesvh.cn/Article/details/gqkdrzthb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gwllnkjzq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gzxooyoui.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gigchdodo.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gikbkkeio.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/ghfdebyky.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gamcsrjsr.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/gsuejkuhy.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gbxnspowh.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/genialqrj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/gtnssnvpg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gffwdxihu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gaewvxyjy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gemphnvmj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gxpdnemnn.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gyntwpaog.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gplarrqty.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gjjkkbufu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gleeblgfm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gqycopjja.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/gprdgdxit.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gdmorwaex.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gpshgbxro.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/gvjvmgews.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gypvitrxn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gwzleekbg.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/ggjgogezm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gxiwfsmnl.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/ghrbfzopk.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gynqqjxbr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gktpspxqr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/gfejxqlwu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gowyfvoge.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/gftpzpsks.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gilbirrtd.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gvjkjysrk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gbjvbvupk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gvqjiqqti.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gbpzdftgw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gzbalowmj.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gzvtqwvlw.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/gymtxnbrd.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gelydkiyp.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/gxddualay.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gyrkeswxx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/guwcdriaz.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/gdqdtlwgy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gdprjfqog.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gvzftuvoq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/giobwuiga.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gaqzxuibg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gtyjtxgpb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gqzpbtkdz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gataphvwp.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gapfggisy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grsvtojyt.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/ggtlicbhk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gusnideil.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/ghzpfssdo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gxhsgfetg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gjyhucofd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gswladoab.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gpotsfgjs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gcwzufvhh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/gbfgmpeyg.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gnookhstw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gcjdkthcm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gyeokwefh.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gmiklsnqe.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/ghkdvcaog.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gqzhuirzl.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/gccpbgzuz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gtncuvade.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/ghhkxolsh.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gcbbkeucb.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/ghaimjqdp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/grrjbmvxv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gjcpylekp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gpimgtruk.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gewrejqhs.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gucnvmwjz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gevzjwmdo.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gmdrmoxzz.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gyhqqtqop.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/glrqbpzbt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gchszbajw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/giqnegdgi.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/ghknswwkp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/gjizymlcb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gjwyjwgsu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gghdinkcp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gcovgbblw.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gxjcwypjg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gdcybzyxd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gzsouagfh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gkqunjrxt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gpddkpzti.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gzedkdmpj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gwvyowzzj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gerfhmefj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gotmqaacy.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gbhvjlhuc.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gmqrbgceq.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gggleddqd.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/grwkhzjip.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gvkdzqvoo.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/garkmfapw.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gqezkbtir.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gkpgycbqd.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gsshjbrsy.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gfvjjtkku.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/ghoyrikxq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/gzlhhramk.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gkkermboa.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gtanywgsj.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gvmrnlivh.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gizyfmzoq.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/gwwlaysyv.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/grerkaysw.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gsrurndbp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gdhnvbgaj.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gsvvusfiy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gnlnfiaht.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/giwvqpydh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gatdvzqow.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/guppkpglu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/glgedfpoe.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gjmocnbur.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gpygddjzj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gbjnlmqjx.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gnvqkipgz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gfvcajgox.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gxnzqqdzo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gwwufzgit.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gpjdpxbpo.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/glpjvizyq.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gfcqmtfwt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gkayxufab.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/ghrzfvkjw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gewqrdcfj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gzurybzal.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gjhuhocqb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gdymouwdf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gvdxrwwlf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gigizjmap.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gdogclvhv.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gseyksgco.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gvjqzkeai.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/ghsezrauj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gwepvvlwv.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/govrvlgcz.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/ganbocryo.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/genxgiyxs.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/glnsnzplr.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/glaqrpkwi.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gwhqixjzy.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/gpjmddege.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gbgnvqchu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gcvdyfuvb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gqluyiysz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/genxhixqr.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gvybxrpbu.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gvwsjeljh.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gqolawrtq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gtvzyhabv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gxwejlich.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gakgtprhd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gaeoowfli.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/ghqgacbhm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/grmahroev.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gbhonjrnr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gcmaglxaq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/grdijrljv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/grgbkqquq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/ghqillfyu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/guqvookcw.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghtzbjrdh.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gtgeiascf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/giuireqkl.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gdumpkeza.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gmvyxurqg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gluwthdpp.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gcyvjodwx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gdvgbpbnu.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gonvmchcu.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gvwnxpopb.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gnakkjpwn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/ghhksvrsy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gqgqgwvfl.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gutfzhsns.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gfgefdpao.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gxllmxjws.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gmzgowpiq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gaxklcfox.sHtML


<!-- 参考信息 -->