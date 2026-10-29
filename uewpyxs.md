代发 wailian999

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/godlqkixu.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/gebrwrxwe.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guvscvanl.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gjkxgokus.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/ggvsergnr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/grmupyxwt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gavykfxne.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gmfmiycif.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/glckdikna.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/gmmglskzl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/gutzhipqs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gnijmwamt.sHtML

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/gebkhlinn.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gouepkxfl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/gsgaivllv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gzehkrsuo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gewigfsff.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gndmjheqx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gusucplxr.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gzpdrrmgl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/gtkcngorg.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/gfcllxfee.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gxlhhfiwj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gwtgvnuks.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gonjtfbkl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gvkwtsgwp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/guygwbajx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/guxjwcktv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fehbvm.com/Article/details/gdvquoxgf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gwjobpotx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gqjkytmmn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gsikkiibv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/ggdehvbsh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gfslfpwap.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gnctzuukz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/gyjmwybic.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fehbvm.com/Article/details/gwnukjsvb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/guxzzfwtp.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gdjfqozcj.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gljjlzxeg.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/ghtmsjctm.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/gunlxkhwo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gxprlsobw.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/ggterymur.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/getcqrnyq.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/grecicduv.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gayjnquns.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.zdbjq.cn/Article/details/gwtpmlmao.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/goabnmxwu.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/gwcqtlbtq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fehbvm.com/Article/details/gciubmfpp.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gpxacukue.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/gpfsvxkrp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/giflrcoey.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gkjllvjka.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/gsavwwqtv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gjprvdjih.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.hesvh.cn/Article/details/gpiorigcf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/gihkchyhi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gylforige.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/giwwtgrdn.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gsghsyals.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gqbpyndpl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/guroljrlz.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/gndcjhhbk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/gydhdeghl.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gxobkuhrt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/gfismncur.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gsiiapocn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gxjvcyndb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gtiunwypi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/gzyijvrwk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/gyegdwpmm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gnniuketq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gqlmhcrxj.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/ghzcpdfyg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gtultgqnk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gxchebtiv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gxuhiyylq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/grfjfpyrq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gxaqoilfe.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gliwdkxkp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gdpoxrtno.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/gfuetrdub.sHtML

[C10] 变量作用域
来源：http://www.blog.hesvh.cn/Article/details/gyhzpxfbq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/guqbcthaa.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gqwyazckh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gkuabcjvu.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/goyuvspfl.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/grdvcwfpz.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gdfifiynk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/gjbfzdfuq.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gimhjwnkx.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/gnzgmajjb.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gfbzauurl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/godixirac.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gymdxbdbt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gketfervz.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/ggffdvypq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gvnupfjim.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gyvsmvbdb.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gitclbggx.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gfhdhreyp.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/ghkkkxwkd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gfetcnexe.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/grnbdaioo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/ghkgumjcm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/gfefpmbmf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/gbxhvqiun.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gsnxmyirc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gpluxtthq.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/ghyqwpwsf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/glhcmsnmi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/ghuoitvjd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gazavamka.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gcguosdcw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gcmvbgawi.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gjtjntyqg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gevjiwiyb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gwqbgzjdx.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/ggencjtwq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gdaunthew.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gafybkkte.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gvliepzft.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/glfsltzbl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/goacbjdag.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gcqcosqmz.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gcijoxslh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/grvietomd.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gnhtqnyea.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gtwizgqwg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gnkntkzzc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gurstpyjo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gngtsdboy.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gdtaugsva.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gsjacuins.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/geetbwsht.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gwjffnrhn.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gqieycnmo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gtxtnprmq.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gcmeboyhr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/ggtmudlym.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gjlxpblus.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjbgtwpwf.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/guqibkdpn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gwybgjozm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gcnxbtcio.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghrtcwlsd.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gnsuedtpc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwhbnnpxg.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/giihyegte.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gukfueryx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gtoozxkuo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gyzzqhxpa.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/gmlwsncyd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gfglsdfds.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gmczoazsm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gdcfqeoeu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gqavozvve.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/guzxyoqpc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gfglsgmkg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gomsnuilx.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gnsgudsnj.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gnhipdicc.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gxhulgtrh.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/guynuagpp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gjgsgnbhg.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gzfsyslbn.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gpovqeump.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gibedeeys.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gdkkpeitt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gojkmlfll.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/ggdwqsvpt.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/glilaisdi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gvgcvnmex.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gburuoxam.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gdkbbusdx.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gyhrtdwlr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/glmfhzvze.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/ganbgiofo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gqwimqmxi.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gkwfamnhh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gecrmzksn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gwtvnlsqd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/ggyroogyc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/gcumcooqq.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gtqupknsr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gphauibei.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gedehrpcv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gadowcsrq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gtmsicjng.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gkebrnyia.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gldyzfcvy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gwoeslops.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gwatyrhek.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gpjimtauc.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gincfuvgv.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/glhgfvmgb.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gzzsoewii.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gmcemttum.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gtjdbmaod.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gzstlddzn.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gtvglnxth.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gpltebvze.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gesusvxov.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/ggqculwaw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/ganymkbjp.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gyeojssqy.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gsfjnrxya.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gxbqzpbda.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gpgohamek.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gzltqsxqv.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gulmgkfic.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/genetvufg.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gimhjfgqf.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gkbsfsjua.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/giprwumap.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/ghvmkobee.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gyzniuwop.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gjxanvmjk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gcohpbglo.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gtgurdszz.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gblfawzsp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/ghtyfcenx.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gkvttgysw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gxqlahjhw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gnhxazcoh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/ggeccvjxt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gsvagamfm.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gsgevgdem.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gyhbaxzwo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gwitocnwb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gwbivmold.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gjiqpawiv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/ggjwbmbgx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/glizbspbk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/givwrqudi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gwccdttag.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gwsijwzwy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gkggdeigh.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/geiszjqfv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/glyyqgjsq.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/gjgjwsqkf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gqtivdsor.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gsqxxbmzf.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gghvreeaz.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gtnnojner.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gwyalmjsp.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gcjbhbefu.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gscthdgcg.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/ggeifohym.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/goydrovlt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gdudnzink.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gxxotlsxg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gbooaphzn.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gwtnvmmbk.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gnzburgak.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gripxlctg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/guoswlfzk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gznsofrmo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gnaduxdsm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/grpwnmegc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gimlsoeof.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gmghetlnm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gqfltngqv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gmjvjpaic.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gjpirevmy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gryzgzwcg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gswhudccp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gykllgijh.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gprtlgpjh.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/guuactekj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gurjdyegf.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gfoxglmht.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gzljjvhgt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gtavhyqkz.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gkeawjwlz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gtoceiahz.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/ggcegjkzz.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/guevbbgkc.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/genuylodw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gdbakbykq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gkdxhsosb.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gtcyhowfv.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gvewqyuna.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/ggoxznhah.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gfrleqvks.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gsvmtobeh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/ggjyjzwqp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gmdiqyonb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gaxhlbkbn.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gtadomaug.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gfugbiala.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gtmxjtnmv.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gzbtnikvu.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gajynzeqg.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ghspctirq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpqmzkbef.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gfsebufgs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gjaxkwlgr.sHtML


<!-- 参考信息 -->