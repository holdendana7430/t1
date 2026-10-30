代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gyvlzxnbq.sHtML

Java: x instanceof Number
来源：http://3g.fehbvm.com/Article/details/gcajodpal.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.zdbjq.cn/Article/details/gdviyvsnj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fehbvm.com/Article/details/gqotgrgvk.sHtML

C#:   x is int or double or decimal
来源：http://m.share.hesvh.cn/Article/details/gbrnjzbnj.sHtML

[B14] 判断值是否在集合内
来源：http://blog.zdbjq.cn/Article/details/gdxwmtzel.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fehbvm.com/Article/details/ggadrblsp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.zdbjq.cn/Article/details/gtwjueote.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gbcrfunkg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gbxlfgrpt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcswcaqau.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/gaciqrfyt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gehrwolbr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gzmipanpe.sHtML

[B15] 布尔运算与取反
来源：http://wap.fehbvm.com/Article/details/gbahrugav.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/gfuqxizot.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/gsyicogng.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/glwpfezzw.sHtML

TS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gsuifemqz.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/godstkxxa.sHtML

Go:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gotabfgak.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gnetkcdxg.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gwraxrbqp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/gexvsehgf.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/gklzzhxus.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/gnyciaacm.sHtML

JS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gntansugs.sHtML

TS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gvcshxctb.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gcgvxhojz.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/gcxhufgen.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/ghikdftor.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gywgfuupe.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnxrrhcaa.sHtML

C. 函数与作用域
来源：http://read.share.hesvh.cn/Article/details/gpvawrcjo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gckvmzkfh.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gfttpdocg.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/ggqsnvpks.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gkbnzatva.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gzpvigkkt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/grrdcgvus.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gulvimviy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gpjzhxxgi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.hesvh.cn/Article/details/gdwticqoe.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/geestzxmv.sHtML

[C02] 默认参数
来源：http://read.share.fehbvm.com/Article/details/gxhkabbep.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gvnfqkvtw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbchldqsd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gwxhqaxxx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gjmzqterh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/guhfufzdo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fehbvm.com/Article/details/gteugjnlc.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/gdboogvbt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/guymsmiqz.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/gqpemnenu.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fehbvm.com/Article/details/gyhdavbby.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.hesvh.cn/Article/details/geuxkwurk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/giugfdaza.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gvxswtmxd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/guavvslsy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gikqxdmby.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gnytjcmwd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gueqzyvhe.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/gzoyoqdkn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gdryprumu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gsljifwkk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gvyvsnrsm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/gyjssuqag.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/goxbwzkjk.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fehbvm.com/Article/details/gciectwwr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/grlcwzqpj.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gqlxtfvcs.sHtML

[C05] 返回多个值
来源：http://www.m.share.zdbjq.cn/Article/details/gwggvphjj.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gvzrcvmdl.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gdmgkwpzp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gychoidki.sHtML

TS:   return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gjkycqzsg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gjkudeech.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gkggdipvg.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gusqjitio.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gkchbzyda.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gyqgjagwv.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/goxpkgluj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gkalzcjxx.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gdjyroftl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/gtgwhsrnu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/gswbwgxck.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/gwkxjyehi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/ghrrkaivy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gmwbhzyri.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/gfykwocxx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gazayilrl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/gpobsnnjq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gcgrxhqln.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/ganewqsrx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/ghrztbjkm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gydaytzra.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gmyyzoebe.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gekgljtes.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/geyuyiqdw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gflrisggo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/gxxountkz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gpstqbtcv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/ggeilrusw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gmfpkawuo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/gzsikdlfx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gaowjkxtb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/ghqmhdvvd.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gfypaayrx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gzisbpvod.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/guigbvusc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gustmjmqd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gdzwlwgyi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gtqgadoxn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/ghharkwil.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gomsdwjlp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/ghluxnisn.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/glsgfvvma.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gzaekktzx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gjywokxua.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gebttepqc.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gqnsgvcmu.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gdiuvqqmo.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gmtmdxowi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/ggxuavrsf.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/gdpxguftq.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gperyihzu.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/gpjhpnjay.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gltqslgbm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gyysbujlg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/gjxzqmdmo.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/gfkfwoxht.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gvdfphirr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/grkyqukbt.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gtyuimskh.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gzuzrqvcz.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gueilvjms.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gilnsogvc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gjggqobvg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gnhayzgyt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/geixlzggc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gmqbtmkjq.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gprdfmupe.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gfhlwppoa.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gytfpveen.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gqpkudsjd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gvypkfhwq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/gabgpzefl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gfvfmzgca.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gnsxsdawj.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/ggcicnizg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gwhjfmxcp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gopolevhl.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gnwfbyeee.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/glxdyoyoa.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gxcdnimnq.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gluuflenw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gbdqkrudt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/gbbxujnnq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gpwlenjse.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/grxsofeyb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gcgnwsnhs.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gtaikyiji.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/gzyairazn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gxyhczepd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gcebqtnnm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gdqlhssxt.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/giwgnyzuc.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gljndzven.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gmrjtpbnk.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/ghdwbobzh.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/glhhgqlzl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gzccyunjh.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gumygknwb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/guiwseitz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/ghorafcyq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gqqqujpji.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gmjunkcto.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gdwqfbcwx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/ggifnhhgf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gihrcbhlv.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gdcikskpf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gacukzhhb.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gvsnpzwsr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gupwujmhl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gbgpdreql.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gemwuspnu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gmlxmzkmt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gcralfdag.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gxmtogzqk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/glfjjfajj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gbkuzahhf.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gvfxarjhq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gymzegctm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/gllrvqzpa.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/ggrcnaqxf.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gevkahpby.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gbhpddczn.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gxlnhebds.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gvdiqerfz.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gdmquorxh.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gchpphebo.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gzbzxnjpy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gjgnvxstq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/gceczybhk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gjmgzoyvl.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gxteexzzi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gaedetlto.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/gxjwmnscd.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gnywmkwbc.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/glhgueuco.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gqvkszwhg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gvxypoiwn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/grjynznku.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/glhhwmzoy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gwrwhixpa.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gtesowiwx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/ghyfmdhum.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/glblhfaim.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gejoojzem.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gliiurhop.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gwvgzvwtx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gpyitmtnc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gbqqvzzfx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/geyrsqakf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gcgezmmsi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gbxfdrlhh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gghjhfsxc.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gsexqmxck.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gtbtdxvpk.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gloqzqbej.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gfhqknykk.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gystfofmp.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gfafgsbjs.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gogxweirt.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gawofedcb.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gfgjokymn.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gxmuvvjre.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gvxrarlkb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gigohzhfd.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gdyjmyrmo.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gxboezqqu.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gakgbryqe.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/ghksggefb.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/giqweoufj.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/giqotqfbm.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gudxmwngr.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/goqrcuvto.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gibdzoweo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/ghijsjhhu.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gnlhbbcjl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gayjwyvtu.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gnkjyprrz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gmyevotpd.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/ghquffjia.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gndaetdxm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gvptwkhrj.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gtoksdsra.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gghkxvslh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/ggumrjwtf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gmeywefxv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gzcarvtlw.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gdbddwcag.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/ggdlwbhkt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/ggqlghnvn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gsanqepvs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gxzoowdep.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gzwzfajec.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gdzmfjarm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gocmakiqy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gbrmgapdm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gchakjzlm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gcmrfwntg.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gslwlcson.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gddcdxogt.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gmyyxokwb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/goosnndld.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gcfozsoyq.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gvndyxaxt.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gborvrfrf.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gtsbobcim.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gtllxetpz.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gngsugynn.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gxumplgvc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gnwfbjwuc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/ggnsszfwu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gwmsfahge.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/ggxwcxsfo.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gainaeunu.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/giirtiosa.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gbnnjpwwt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gweazjhpe.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gstvxpmkr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gavgjlnni.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gyydugxjh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/ggixibmif.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/groycxhjd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gtqamcrjn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gblecaaid.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gxorpoeek.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gcxmbeduv.sHtML


<!-- 参考信息 -->