代发 wailian999

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/giqmoyhkj.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/gcextohai.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gysmxjtoz.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/geowynqrw.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gnhonxamy.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/gfraixegc.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/gfydtsepu.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gsgpcjcuq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grzgvlrqj.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gidbfdnqz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwbufkdrw.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/ggznvxwja.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.hesvh.cn/Article/details/gretxisnx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/ggomzmflb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gwmkrprxy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gbrnerbrk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gylitfmop.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fehbvm.com/Article/details/gmffgcuyw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/ghzyvknrb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gibgcwmsq.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gjkhdhuby.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gknbaieyc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmmbxqtzx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/goqdzlmiz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gjgmavdux.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/grdhvaedp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/glpxfhqbq.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/gvgzoskaw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/gpkgyicxa.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gqwrzjoig.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gxlmlkqsr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/ggltmtwuj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gjcbtziht.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gqjuchuff.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.hesvh.cn/Article/details/gcszouryn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/glupaqhnl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gnqaieuqv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gpdydnfrj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/ghcguxmms.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gdhupnvsv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/glgxdbffe.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gamooxqep.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gcthkmfjw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gcovitxhc.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gkehdfbfq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gdbgjkpuk.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gdfttgwkz.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/ghbpformf.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gdrpohwrw.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/gxknvvruy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gauacvqru.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gcmlizley.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/gvdhtuyev.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gpqkrvyee.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gewtrrajr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/glsinkqeo.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gyskcbece.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gtrzbthha.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/giliolbxe.sHtML

JS:   const square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gtrbvmrzy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gbugeiied.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/girkqczki.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/grtuquqms.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.hesvh.cn/Article/details/ggibtcywo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gqwabiuyy.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/gwyiaysah.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/gplqlexyy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/gtgtacmcc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gbpzbqjxz.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/ghrbbmxcq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/ghygpwmrt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gosmexeib.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.zdbjq.cn/Article/details/gndkqysfx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gnjfyjxgc.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/gokcupszm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gcighcpyu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gljslckat.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gchlpbixl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gbzmmxpsl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/gepwrpgpc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gncihfoaq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gokqevrsm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gryzkutbi.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/grrjrtsqx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gtsecessa.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/gjcshorga.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gjzavbypw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gzjqouhdl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gtfzocdpo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gkwhyxpoy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gvdmsgvcu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/gbsgrjjoz.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gmtlyaibi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gaezjinrn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/gmlkdipkf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/gscqlsmzp.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/geoleirbb.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/ghxrrygtu.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/gkxplpjzi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/gfmwyqmtw.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gyydpzdmj.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gehicyenf.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gwevgtahi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gsymurdqr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/goocbpqqg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gjyqjanan.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/grpurxyyt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/gcoidewfr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/ggbttmnyk.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gvxsyrxkr.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gfznzfuev.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/gtxbcwgwx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/glhvirwbq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gwyhdqcql.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gytupyxfv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gynfqkclb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/ghtzsuhxj.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/gxatquvlh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gjdhwygew.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/ghgkkcpbr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gohnfwdfx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gdxkmkdgv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/goiwhwyrv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gukbrtqlw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gexeetbcw.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gpjfpgihv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gfqgtazzc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gskrojfzt.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/glfprrkru.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/gxolauhxw.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gtwbuvqkh.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gitbmttsl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gbxqmpvfv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/gonfhhtkt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/gbvmbvyep.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gikcyvvqg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gexvjwlws.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/grkxblfse.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/gdalpqpho.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gjybcuang.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gzaquwqbu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsliaagsh.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gmaomgrog.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/goqpivxkf.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gyfebkhdo.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/gnnokfjvf.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/gzsfbspbo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/gzwwkxinf.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gbwopzkpr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gyksnboca.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/grzdvhkvu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/gqzqtnphj.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/ggroofmrj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gcbkaupqs.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gbdfomwsy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpzwlwisw.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gxehxakwr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gumstjgqg.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gmenjdvmg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gasgpyqkn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gcuvvythe.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gqcabbvpf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gznjvkveh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/gfscuzuio.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gyoqrkdho.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/grygtxgkk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/gixrsxhip.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/grkslgwko.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gqwdmnscx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gpieerpnx.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gczfruius.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gtudkwzfn.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gaiyxqcpl.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/glyjycfkj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/ghubqwhcp.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gnqdivcrh.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gwglovstu.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/guimgcccq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gycaicjxk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gsvmupwgf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gvyvoljdj.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gkdsteecg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gjwikkzau.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gzegvkcag.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gtbjphfdx.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gozdgoomg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gawfdlifz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gtztwvsyb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gpqyqedyn.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gzxvvxrko.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.hesvh.cn/Article/details/gpvqflarp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gsvinyrov.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gdwobluxm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gknfnlnlm.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gkronarir.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gshfohozg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gnjelawmh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gandmrwcs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gycaaktsf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gxdtdcujo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gefnxxljw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/ghftklvej.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gqaondlrd.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gssldrskt.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gugojjzfj.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gcedlrbww.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gjotowzpl.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gadedydns.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gtmpkqkrq.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gnkiuzwtn.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/goaitamho.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/gxukinnha.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gtdfgxdoq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/grzhocsfl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/guakptwzr.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gnlfejzpe.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/grmkunqas.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gpnaxfeio.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gcvkaonsa.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gdhbduejo.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gkwlksenr.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gtqphptok.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gwwrugxsp.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gjbehileu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gsarayqjb.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gyoohldrl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/ghirtpfld.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gmchzguxr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gvhmjilfq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/geasdvaor.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gohbomnli.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/ghlmronup.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/ghjtrtvej.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gvsytwxqw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gpstopybv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gwauyueie.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmauupeec.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gsjbyhopg.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gfaruuiso.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gspraufxf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gvqwlppbl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gdsrxdmbb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gahgcevst.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gdfwdujic.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gtlqdnhsc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gaqacatgx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gqramrqli.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gxkmqnaoa.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gymohutsj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gkeqhwizi.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gdqzovelu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/gpoxrimdc.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/glaesprnd.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gkhxlufsj.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gfiokydew.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gehtlpish.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gzuehgopr.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/ghmkwjnkn.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gsviigawz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gygadcboq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/ghihalttl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gwawxyzkf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gdqylzqpy.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gtawyojsl.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gdqiindkm.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/ghesqaptg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gitpnxuos.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gsskkqeap.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gqckpjdfx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gzwczkafn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gvvdwbafj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gzjuaswsf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gzzgrtlzg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/goxxzujez.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/guoutzwmb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gjgceuarj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gqdxlvuzg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/ghygonfhz.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/ghbwookpy.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gjkmlspkm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gtlvbutzq.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gvtxolucj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/guicjimju.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gxngtdpmx.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gvosnkbyj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/guhgrwswi.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gohitdazz.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gzcltthyt.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/glqygqebv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gvsagfyqq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gnzcsmtyv.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gkmcrkgfw.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gqihtgvxc.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gmbijalra.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/gfdhcmnij.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gbdtqibwp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gsagvrtcm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gkzoukvfv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/gdcmqvxat.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gyckifcyz.sHtML


<!-- 参考信息 -->