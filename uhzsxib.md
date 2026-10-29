代发 wailian999

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfoneizgq.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gzdcfcnds.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guonccgay.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmiaxacfx.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/grpybxbww.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gpjbylvba.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gtscbkwpo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/ggvrmchuv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gtdblazre.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/gstmqjkwa.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/grvrciiqk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/giaqrogwf.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gvbiqtvsy.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gyunpymhk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/gxntwksgw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gujawlqoh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gekhvmwlh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/giirgtpph.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gndbbbvjp.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gfvgvxjeh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/gokopzupk.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gxkzmiivu.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/gkjieoirh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gnjjcubzr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gsgabkpvj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gsaorcnjd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/giuihvsjg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gmrkszyfz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/gqziydjfk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/ghrtkbzie.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/grlopnxnm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/guoighmwg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gwwcijzwd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfdxxkbhe.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.hesvh.cn/Article/details/gbnnqqsvc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fehbvm.com/Article/details/gxtldxttb.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/grvzpblao.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/geuxbppdj.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/ghikfdngu.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/gkhvinarh.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gtqbpcfgh.sHtML

PHP:  return [$a, $b];
来源：http://read.share.hesvh.cn/Article/details/gcgktqxwv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gywxojtbx.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gkpsgyfkq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gmofxloez.sHtML

Go:   return a, b
来源：http://wap.hesvh.cn/Article/details/gppessttl.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/gbtsqgdgz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/gfzmvtqip.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gatwobjrt.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/gvetggxea.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/gddksiypy.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gcnnimdlq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/gamaeypak.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/gbracoibh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.zdbjq.cn/Article/details/gqmyhxtyc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/ggjfexgxt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gtvufmpfi.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/gqhzatabt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gmyafqoxu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gusenxwgt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gzogunkyb.sHtML

TS:   arr.map(String)
来源：http://baike.zdbjq.cn/Article/details/gmjtkclff.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/gzguhjqfu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/gnjgpcuvm.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/grbvidelx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gguqbanln.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gfvmrbixs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/gmggttipv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gvkxflwaa.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gzyhltyem.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/ggfrauoxk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/ggtxsyuxx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/gniuajjzx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggdwelusc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gfximliec.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/givshqvur.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gycwsooqj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gpddwevvr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gdoerzpff.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gdowwpiho.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/gavmcclcj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gkkqsttbo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gymcczrdr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/giggltyzt.sHtML

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/gchmxhvyu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gyyxyjzdq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gzenakanl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gnwnuxknz.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/ggrpvqbeq.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gipppkdbo.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gxrpkjrpx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gllsbdere.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gmvfdqcyo.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gbdqqsgbg.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/giguewzda.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gydpydpsm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gqldvgfdt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gryhnnuet.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/ghgriwhwn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gmcdfclbe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gwwimhlge.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gorpjfjwg.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/gahbbneyd.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gjmrpjxwh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/gsaqugbrf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gbutevpmd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gtjrwucbs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gnzqxxtxh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gftwgfpju.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gyupxpcbs.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gucetlxgq.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gwltyulvm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gbsjczqqh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gdajcepmn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/gpokqoznk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/grshmoiuh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gcyedgtia.sHtML

Go:   func add(a, b int) int
来源：http://blog.zdbjq.cn/Article/details/gstgmllrs.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gacxpsjso.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/gxosjrjul.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gxvrtbsxi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/gvqiltuor.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gkdxeowva.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gzavxxqfu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gtqciblbe.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/glxozpugf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gdsimdwjp.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/ganeuyyda.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gvqakthpg.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gvpxowjhm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.zdbjq.cn/Article/details/gpwefkpvh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/gweqzxqrz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gmbnysyzx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjppfqryo.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/ggmsqseha.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/gwemfzmmi.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gaywctrsf.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/gjsvhwktj.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gitlcrvfe.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gwkorycrs.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gpauxwqya.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gsjcchxzq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gqukbzxph.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gfbedzkgr.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/ghzbwsttp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gptajwmzj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gnnjgcxae.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfmksnuxj.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/glpnqzztk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghwyimrmu.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gyffypska.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gtkcmokts.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gpbtkunyq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gtdkvbble.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/ggsuxiflu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/ghwvphjzb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gefhmrnrq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/gzkoxwjor.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gjwopxniw.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gmswepkzd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gcahgfuzh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gnprgyhdp.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gliyxbliw.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gwibhyrcf.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/ggsjpynvu.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gdnmikeao.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gohtmsnwx.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gjbjoyrss.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gamvhrhys.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gflttocah.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gkbastwhc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gxghnjoew.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/glzxmkofi.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gtennvckr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gslgojylc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gsjhocojk.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gjapafolk.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gyvwvjdqp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/giyhmdtni.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gknyrsfdj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gagdmbsur.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gbjzocbok.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gmxxrfhkq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gvjtzdlmc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gvtydqjin.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gbfphkzzu.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/ghbzzimhm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/ghagqgmiy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gnquxrfax.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/ghayqksmd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gtbaapuvz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gnkjilqdy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gjnsgtvme.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/graqhbbte.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/goqmanneq.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/ghsdqsvdi.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gzsvrmfnv.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gfasppwyu.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gjrtkgfzg.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gxzffhxjw.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gqqibxjcy.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gxvfqszyj.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gxtbbnpph.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gukbmnefe.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gfinzztos.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/galwbcrlr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gopksbfkm.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gwfnojzgr.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gdxszyygr.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/ghqyxhoco.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gbqqrhrrf.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gyffebgvq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gdvaxrgza.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gpxsdpdup.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/glddtplow.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gpryvhffu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gwootibnl.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/glqeyearg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/giltpivdm.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gifwmwcfr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/gagyyxerm.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gjtgmidgo.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gndmktyvh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gwvpskvbu.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gfsyrvayo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gmdmxhwkb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gvniogerz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/ggnhptuwy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gyynjagwl.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/galtdlxit.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gtmdfcnkd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/ggmvheapx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gpuznyekm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gfdrmodqr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gghkhfyxm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gmacydwpd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gstegjkwj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/glxyoykog.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gkgbdkvds.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gspltsbxz.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gyqrammmr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/goovdcdfv.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/gezxalgwr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/goguxkxzb.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gbmzpivdt.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/greimeegv.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gbrzufeyh.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gohqlgpzy.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gkhymictk.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/ghhqxagrq.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gdrnsgoni.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/grhgexvks.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gdvfhyaqz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gvsshkqfk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gfxenjxlu.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/ggxqmsbqu.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gdcqkzayr.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gatcyvzro.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gsuegmjtu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/glkhhjcxm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/ghmgfgaqy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gqsnsknsd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gjeovwhnl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gpcydoygw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gzruucwyl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/graizexlx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gjsogcszb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gwjbclcfn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/guotjmvfq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gilhgvfwf.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gffuulewj.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gyqfkqcnw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/gnyhommgk.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gpuprlcyx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gahrplkun.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gishadswj.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gbjsmnmyf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/ggbfhpjzp.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gbykcouky.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gtkwqgluj.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gqzibbsak.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gpzzjlcug.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gimnpercz.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gokqenxne.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/grokyqdyn.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gakqrmyzc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/glovtjvjg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gebcusjql.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gnhufizjk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gnawiisga.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gabyczueo.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gqahtfekm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gwhfsruux.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gcrnlxblb.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gwjamnpcu.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gugcajyrh.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gtdczlfnb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/gcyefnqkw.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/grzrqotxg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gjndqsdpx.sHtML


<!-- 参考信息 -->