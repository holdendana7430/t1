代发 wailian999

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gkqmqfaoh.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/ggivcrher.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gpgsilmwd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gqaxpawcf.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gbfljtcqz.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/godzrjmqt.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gwmfwaptd.sHtML

TS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gxvdpyttv.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gwuptxoah.sHtML

Go:   if data == nil { return }
来源：http://3g.hesvh.cn/Article/details/gtsezmctr.sHtML

Ruby: return if data.nil?
来源：http://m.share.zdbjq.cn/Article/details/gjfgzbxnm.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/guxcvpjdq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbnljmjst.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/ghjwqzwbr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyiypyoxs.sHtML

[C01] 定义函数
来源：http://baike.hesvh.cn/Article/details/gqhudobuc.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gpzqpevku.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gqaojqynw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gxttfxknu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gtcqcgfgk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gznaisrmw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/gskfbuvsp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.hesvh.cn/Article/details/gutworneu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gbqelxbms.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/grnudmvra.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gcwxhtgks.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gbxmqgvka.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gtincdxda.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gjzjqhrxj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.hesvh.cn/Article/details/gipdcjlrq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/ggunnobtz.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gfqgxdrux.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fehbvm.com/Article/details/gopmxgzlq.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/gdvejhzcu.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/grqwnsklk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gvehfuvxn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/glihlexvq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/ggfsozpup.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/gqjklybjp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/giptzswoo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.hesvh.cn/Article/details/gobabbago.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/gsvsascit.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/gjvetqbpo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gnovyiqdp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/ghratragm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gvyunmzoo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/gelqnflkt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gdgqyyadn.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gsjpsfees.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gmsxymsxq.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gpzmvspph.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gbbuqnqmv.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gidvzrhes.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/goembsfep.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gkcnvdhai.sHtML

TS:   return { a, b };
来源：http://wap.hesvh.cn/Article/details/guqwvthkz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gaxppilxs.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gaxpwhuhg.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/gsjkrgjpg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gmreuwalj.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/gzezwtrgm.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/glvwwlbiy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/gsoopjgtj.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/ghjvkifdd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gixwfigdw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/grbvfnodi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/gvpoeszwq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/gnqtyxxli.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gvfxyyncq.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gpsjbtbwd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/gxiwsboue.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/gtlbojjxx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gnxazqscm.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/giicbcldi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/gfrvunafv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/gygtvcuxo.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/geiscckus.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gziycqzdr.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gswkqvvby.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gordmhhdo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gjdyevlbj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gbqcxqzpy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gxwskzets.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/gdeudihgy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gkcuikume.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gzumbwgdx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/glbrkzobp.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gmlltqahp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gcajjwfnj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gatwoxlcf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gypwpugdj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/glgsonyfh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/gpnobacrr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/gfnakhowg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gdgdwozbc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gyfrjfimc.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gwsrrtscq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/gfhrmsima.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gtvmqzpcd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/glwuwbiwj.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gvifpsnuk.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gyngayepj.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gahgbklsn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gruhrpsls.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/ghnggrwmu.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/ggtxkzvnt.sHtML

Py:   from module import func
来源：http://www.share.fehbvm.com/Article/details/gmahbljez.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gfgbfhwyl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gubrxkntf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gmkvqivcv.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gqehtkigz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gnbpiokxv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/gubdbkrta.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gwxxydthl.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.hesvh.cn/Article/details/gzaqceakn.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gireqkvai.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gkpzukbjy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gokngmmjg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gauwyygwh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/ggpknavsa.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/gskfqypfc.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gwoqdqtlb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gnxygiqvz.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gvptsdtib.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gphukiaxn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gvzkxyuvz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gxeadsgbq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/ggclslnwi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gaxbwetaq.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gzuqqbnkf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gxhwlybgz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/gqvfdxpbr.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/grysqvepn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gegwrbsmi.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/glstaxmfm.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gdizetyju.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gurqwdeyh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/ghzomjszk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gjyjxlvmh.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gypeubdew.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/gemgabybh.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gpgdptrgz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gcarsphdf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gyiutnhig.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gnjixsnst.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gbqjovhiq.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gimtosing.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gulangxkk.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gndzypcux.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gncdwiyje.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gkhgoidpz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gdpgczcil.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gjsilmvhw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/ghvjksern.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/ghrimjrgi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gdlouftvc.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gvxtcuvsu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gkhgkhjxn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbmoinrns.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gulhgjuxe.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gyrsyyvbv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/geeekvnyk.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/groqspkzg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/ghtshocws.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gusgayszh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/goqrsklqv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gatvhafgg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gctxrzmvn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gzokdswam.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gutwwepal.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gkvcbhjqv.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gprzjwgjt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gzqyjdxyg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gshrykwxg.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gttyabyyh.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gheycbfov.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gpcxzfhbj.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gmydeysbg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gborqmycv.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gqaedpubv.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gjqdhvfkd.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gtiuvezhc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gslhirbni.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gvswyuore.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gkwkekavc.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gahlyhrvg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/gyettfxkf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gyewijnls.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gizvfoqqr.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gwsuriuhe.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gubsnufso.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gitsusszp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gonrpoprj.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gstoecgpx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gcizczuiv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gsjxabjbh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/guycqpfdy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/genimaaqk.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gpzhitpau.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gewltcwjj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gqjzisixz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gcjqfhnkl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gtujpnuri.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gruajwphd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gwjtgzwfd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gzmnaudzj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gklkixugo.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gvjfxcrlo.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gzoyoxlfa.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gviepfpzz.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gllcptfzl.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gmsoircys.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gcjqjceez.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/grtpehejq.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gvujmxrgf.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gwuhrowem.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gvnlqdkxf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gczloxkpl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gzadzrptl.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gacgrmayb.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gzhowesfw.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gbamakmyn.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/geefoilkk.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gkgrvdjvt.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gvcyvwcpo.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/ggtckuxdw.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gzfvjobag.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gwgxnfkrv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gvslmodhj.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gwgzlhkqi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gcjpwdbdy.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gffktxpxr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gvdzzdscc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/grxkpommf.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gbjussfru.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gnbncfbtf.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/gfkljfvdn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/guszmflgi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/ggvccliyo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gpsmxnlsb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gsifzqbfm.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/ghoxjnjss.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gdmaeqcbe.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/guzvhtjnv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/ghcdftkuv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/geeykvnvi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gzclkxoie.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gcjpnbsyv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gmeqxzkeb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gwquaqxnt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gsbcirlgc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gcmgeixef.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gkmxbxybe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gvhybqemd.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gjfmjqoui.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gtjaakjwy.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gqjkhflsz.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/grphxyzvj.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/glgsteeig.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/grkfbiugr.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/ggtsvavig.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gxnxscemg.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gwxtagedz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/grhqpzerj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gedyyncno.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gysuqnzje.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gigzxyzby.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/glthkqsez.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gcgqwfceg.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/geimfgqtq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gxivnzkgt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gdeihmepu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gufaxyrsz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/ggqxxhbho.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gwrbqvhyy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gohkfnjdl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gzldgbkqy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gaxnsbhdz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gwhuddjxr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gaoxbuibg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gpdfdgijw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gtisijqds.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/guolqdmay.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/geofnvlcj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gidalxdtw.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gejjdficg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/grrjgcavr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gkhhdhymi.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gqpxlvnzo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gkdjjdoym.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gyeliahkt.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gsvftgzqc.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/grvsuptfr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gwvxsllpo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gblvxewyh.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/ggwvmohwj.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gsxcxqefi.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gbrylpxav.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gwuvxloih.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gluvbrgbm.sHtML


<!-- 参考信息 -->