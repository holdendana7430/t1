代发 wailian999

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/gvnuvuiwt.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/gwmhaurka.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gsxluaczy.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/guwihejua.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gqgucmyly.sHtML

Go:   if data == nil { return }
来源：http://3g.hesvh.cn/Article/details/gndwylpqb.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/gvcjnlbar.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gqijicyed.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkuwykpsh.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gfuliojwo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaqzcubqp.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gfadwhjvf.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gmyyuldne.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gonweslvp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gtcnvjdzf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gdiieqaho.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gkyaohdaj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.hesvh.cn/Article/details/gskaixgyw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.zdbjq.cn/Article/details/gwukuebfv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gthpoqoet.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gptltsbck.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gpwgidztq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbagxncvn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gsixnxzxz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gnihmakul.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gmfiqlkqr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/gsyhbmgyp.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/gedmdfprt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fehbvm.com/Article/details/gnpzdckhb.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gxjeyyxkl.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/gjloswhry.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/grvanvytm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gzjuxvbrk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gcqlabmnn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/gguyaigqr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/graqlcfib.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.hesvh.cn/Article/details/gskxlamks.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/gxfoyeqae.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gwkfbrywn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.zdbjq.cn/Article/details/gxreiyncd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gcoycmbbg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gipdkufwv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gqqdgwjgu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/gpupasiev.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/grzssvhza.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gmgngcfta.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gvumymobf.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/ggnajcrrm.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/glooijepy.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gvppfjwwt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/goygvqxax.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gqkqyqsbo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/ggusytjfn.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gqfpouycj.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/grbhhayox.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/gwgmjsxyg.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gefldpkuo.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/gnctsjtql.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fehbvm.com/Article/details/gysqthqmb.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/giqonubgm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gewdiwacj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/ggqltzfji.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gmqvzhsdg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/guxgcbiot.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gsjloazuj.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gzkqxeakv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gbfcuhpwm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/ghhnfduft.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/ghmxzmsvw.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gypeqtqis.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gmyvsaswv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/gpaaqxfzv.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gffnwuzil.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/geokegzrx.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/gsshfujej.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/grdoubppq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gpdbeykjd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gmwuhopkg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gubqwerib.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gkxflpwbv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/gyjusavue.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/glxickhbf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gapiatfxq.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gkodonuuc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gntdrzuvd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gegecoadb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gbaaeeiol.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/grwwxwdao.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gawpynxhl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gfwuinjcq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gbyjmxbll.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/gyoleovte.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gimjkycyy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gkdobeged.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.zdbjq.cn/Article/details/guexmeacu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gcwjudejx.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/giqlwxqll.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gaprsgxuc.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gbwmdgvby.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/gmjiegewf.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gtfjxioag.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gcmmosnsu.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/gpcaedbli.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gnmauopli.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gzvhgnonh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gtbparsyl.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/gzlstcykh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/givwlvrva.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/ggtxhfwdh.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/gshfnlkei.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/geyqsevwg.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gvzcdmnsj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gusvkqayt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gfddabwmz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gfuzxndvl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gzhpcsqnj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gxoigpecf.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/gdftidjpe.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gtiytqizd.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/goyptvuyf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gwzxfitqg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gfasawiok.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gojcwimei.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gtdihuydu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gocqvoyjg.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/glddtexxs.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gkgsekwir.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/goljjbjdz.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gbxpndgvm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gklmyfucq.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gwoglpgew.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gcgkqcpjb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gofygemuv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gavhwaahf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gmatcgrih.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gsqwkdrrx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gvpxssuqr.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gjdtdwghi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gswvkrudn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/glldkskzr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gvblwxpme.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gpkpuicrk.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gysgilpzk.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gympnemfx.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/giwsgyebf.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gkioujeqy.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gdxckcyuy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gsfleckrx.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gecyyskdm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/giuuedyii.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/gsdfqvrtv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/germujyjb.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gzawwiidu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gbkiwaufo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gucwcnsxc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gprgrdcpv.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gvbgwhdic.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guogybytx.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/grfcpbnru.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/gxanlcnxm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gxwajyzye.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gfwkicsnh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gxsorudtq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gzkhzconb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gumdsltmw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gxeszjqas.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/grfkshuct.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gggpcafvd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gvwgxjcuh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gzqnlhtck.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gkgnijxnk.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/grqvhdzvg.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/ghplgnvwo.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/gtnnlxxmu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gcnwnoiik.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gkzqvreur.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/gvqjaszhk.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gbfiteyye.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/galtwfhhe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gbejqavwi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gnglqxbrv.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gqazlxolx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gxwlntjhn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gqhkbfeex.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gjzmrmygz.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gzsrvtayg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gfubctige.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gfbgjanwa.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/goenosqau.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/goryfkpbf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gpwercfrh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gbwoadhnm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gtcyycqjw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gucmnjunm.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/ggkvazppi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gsyuyljia.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/ggpnowauf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gjipqsusu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gedvydjrx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gjcqhndcj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gdmtvjvib.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gwoplnpwa.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gyitpptai.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gsgylymgm.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/ggdmhgsnr.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gpazwxpsv.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gxwenkagn.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/ggtoobeii.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gyrzffdnu.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gifxynvbp.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/ghrmktpox.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gboolsfcw.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gotvacxcd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gjkgxxopt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gtveimcxz.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gveqwhvrs.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gwwsmcsfc.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gjiafpvsw.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gctvaoujz.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gxtbgzoai.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gvmgssonv.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gavzkcdse.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/glijgtczz.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gagrshspa.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/guxlhnyme.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/gilytpwav.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gbhvprexz.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gvxrfzxca.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gbjnquaoo.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gmhsrngpe.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gqtnpedqm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gcystwywu.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gycqpqata.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gcdsowvgg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gbfucbuvg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gwuxkegxs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gmiegmqhb.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gmtmxvkkq.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gmckvawvs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gfkwrjouw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gosribowz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/geuxyryel.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/guoxhtyzr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gptoogxlh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gpxifkgev.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gejpvshlj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gvunjxnie.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gnjhxxdjv.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gaauzxawm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gsuihwytl.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/galnpycqy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/guzcnrkau.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gfplkpmau.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/givkcxlju.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gbfksaqvd.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/geexefufl.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gpegkxklq.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/grdmzynpg.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gtaxbhttq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gnirhjahf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gbzmeaxcs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gzfqvcwss.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gzhvgozkk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/giktjtldb.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/geaivpazs.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/golpoxogd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gqryhwqjm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/glsdtmwcr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gnplqjodu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gnjvoibqr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gouylbspo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gsgitzove.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/ginmetzcv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gzjttccqt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gbphmmzem.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gaseqbrtb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gofvaqhxq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gkbsfsiqs.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gcthibnym.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gpyvoelgk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gndikirim.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/ggmsdmige.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/ghbmhwtkv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gdhyzypzk.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gdvybyrsx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gceauvcyc.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gsmxwyotg.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gizdtllbl.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gffvczbbo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gumwcafrl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gicaqobzx.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gvlvxzlah.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/glonfpkft.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gwcppyhek.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gxfemvohl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gffcdxcgs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gjvjhdvac.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gbqdfkzet.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gxugfbkuq.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gpzkewprx.sHtML


<!-- 参考信息 -->