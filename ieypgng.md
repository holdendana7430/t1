代发 wailian999

[B13] 判断是否为数字
来源：http://www.blog.fehbvm.com/Article/details/ghgillbem.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.zdbjq.cn/Article/details/gqwhftdno.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/glgyzkuhz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gmlxpbloh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gcsxsubmr.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/ggeazvmcz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.zdbjq.cn/Article/details/ghjuonniw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.hesvh.cn/Article/details/gfwfmalzu.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/grlcctywn.sHtML

[B14] 判断值是否在集合内
来源：http://wap.zdbjq.cn/Article/details/glsigokjs.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gmvdaobfl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fehbvm.com/Article/details/glauoraxe.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gzomxvsva.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gqwkukqju.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gdqvajvtv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/gwrcnvggn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gqqqszixm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gestbhwpy.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fehbvm.com/Article/details/gavtdbfzj.sHtML

Py:   a and b or not c
来源：http://mobile.hesvh.cn/Article/details/gymhjcqkb.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gvyzwjpzk.sHtML

JS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gwsndiqum.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gazqedtzg.sHtML

Java: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gkkbkntsa.sHtML

Go:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gcggloubw.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gagebijvw.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gcgvvyera.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/ghqkqptyp.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/ggtnwlpbi.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gaxdytdsd.sHtML

JS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/ghbncfnay.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gaztfbcxa.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/graheczyw.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gmqhoafuh.sHtML

Ruby: return if data.nil?
来源：http://m.share.fehbvm.com/Article/details/gzdjihowj.sHtML

C#:   if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/glexlmgjz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghranqxaf.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gilcqierx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcbzlvdkv.sHtML

[C01] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gqwlteedj.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/gztjgdewq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/ghbszxoog.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gnrqflclm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gxpvigdao.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gdzmezltv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/grrojdztc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/gpanuvauo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gpkvdiqey.sHtML

[C02] 默认参数
来源：http://www.blog.fehbvm.com/Article/details/gzoibkmae.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gdgmeoxnk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fehbvm.com/Article/details/gdgaextnd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/grhczfuff.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gcbscagfj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/gjctpetwm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gmgpjcxyl.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gacpabbaf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fehbvm.com/Article/details/gezihdsxa.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gccqnagok.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fehbvm.com/Article/details/garwmvclv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gzpywqifi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gxriceupn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gfzbizcof.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/gyuvfjwsm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gpkxssleo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gmmyxpijs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/gqcuxzher.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/gvemztavu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gozzxfvpc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/gumarpbhi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gfqjgvnss.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/gmnghoxzz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/guiduxcgn.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/geybpiodi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gebdsyxci.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gwrmjmgks.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gijucvfzw.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gjuavefgv.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gxoaiwoqz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gkhstvnla.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gjeuamhjy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fehbvm.com/Article/details/gqkhagotl.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gcjotpsqv.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gkjtbtpuz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gwzghicoz.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/gwfqnqzoj.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/gczfzuhuz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gdpzabeiv.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gujynzgkv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/guzuimiiu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gxefnafva.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gabxtkqyl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fehbvm.com/Article/details/glfdbxqmg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gbauuwfnl.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/gsfaqqljk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gtjnjhzpt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gfynfalim.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.zdbjq.cn/Article/details/gyyeqwexd.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/gicpvszqa.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/gybuvnxen.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/gfbwlpyau.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/gclsekbra.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/gcfybcdtk.sHtML

[C08] 闭包
来源：http://www.share.zdbjq.cn/Article/details/gnmsxztmf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gnazduwxd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gfzajjwjx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gtpflyeqp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmspvckgy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gzdssuyhs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/gesyolgxe.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/garnrbvmx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/ghfvacmcs.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gxrpdbwds.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gwhaqbvik.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gtlvvrswn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gsbqrivtm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gaytpnnfv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gcmjgzabr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gyvxplcav.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gyomptkuq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gztspauuc.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/glnamrqsx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gdthfplkt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/grgubsmed.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/gvsvhrqmu.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/gcwjumesd.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/gxwrzcogw.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/goljwzfvk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/giymicnye.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gcvlclhzg.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gblaljrkc.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gqvstrhhd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/gnqsxcirx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/grtsezxeu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gwdiljouy.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gwrvicoib.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/gtseugqqx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gymotcpua.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/galaduldf.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gaulvhbdz.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/giyxrmlqa.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gmyuhijji.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gazzihcyh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gverkvyrx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gblothjiu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gssekiedp.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/gfykdjcct.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gdqhbojml.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/gycovdtmn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fehbvm.com/Article/details/gjojapqqr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gfsulcxga.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/glunjjxln.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gihwjtnce.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gvaoxfwmn.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gfelctqhi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gwgvydmpn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gfmzqxsdk.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/gmjeeaiky.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gztezyeol.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gsfxrmwiw.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/grrzmvcxm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gdiwwemce.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gqknawgil.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/gsylukdqm.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/glykksdrp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gfawbfhdg.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gokcoxukq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/ggluafulc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/ghzzhplhl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/giunmmebe.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/ghkojxiza.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gajertmdu.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gdqdpodrk.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gyqbtikhy.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gqsmpuuyc.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/gvqkbykfi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gzsdtyowp.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/ghvlatkvv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/grkvcbbwn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gidwmmiyx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gycqhnqzo.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gcgqrfskw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/glvurucop.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gzpgnjpav.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsrmxpayd.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gcwurtbxf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gohgxexnc.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gxgltymcp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gaatfalpz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gplgqsnku.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gyeqpzlyc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gsqhxfoul.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gathcapmb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gayfqdhnt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gmkkoiene.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/glutbsxqz.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gbuwponmb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gtwhsncdg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gvbqlaxzh.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gwxymagvw.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gxdbbffhs.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gjmkyyekl.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/guyovqznx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/gstwtroqh.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gdblfgmob.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/ghxvkvjhs.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gkdbaduqc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/grgbicrko.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gzmqfsiin.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gmumeccpk.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gmrulalah.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/galhcuzdm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/grunypogz.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/geiswybth.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gmviarqif.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/giqlipgvi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gyplntlos.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gnvslrbxz.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gmsgttgsp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gfgbjhcqn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gfwrxzqwm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gegfvyyww.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/glsixooiz.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/gkfdtfuux.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gbafqvsdk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gpyiwyjif.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gxgbvqmtk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gowlupfnd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gyuuzwbjw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gvkdxikrf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/givsvpvrd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gkjhyhqtv.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gfgajurqa.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gairyfkrf.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gzwvlahrb.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gexbigutz.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gdtxlzrcl.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gkidxgdgm.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gotjybypw.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gtrjxuefo.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/giplojaav.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gcgazawje.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gnowxhcid.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gcpeoxuri.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gdxoeeyje.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gwflgqhkm.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gizqjwsoy.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gjnijkfcd.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gxfifigim.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gepvdfnpl.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gegexqtxg.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gbymbthar.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gooaashji.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gjqnlmrhy.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/gwjhccyfj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/ggivsfmze.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/ghnmckbgd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gsrjxyicd.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/grhnfhlbb.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gwogfutpr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gpmoeezif.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/geylojalr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gfnqgjsbg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gdfzdnhbt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gyvuwiklv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gqjqacmhr.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gnpnqbexz.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gyplejnpp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gsftzdaia.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/goxycblcw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gduiqbeye.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gjidluofy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gpmwhhgqw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gshvasxkq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gyswjsghw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gfblilqie.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/grsazbutf.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/guhuxgkwl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gzlzsqvos.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gwxkvxcei.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gfcfftgof.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gsgafolzs.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/gasqjaffv.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gqztteijm.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gesmvlapa.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gzpfqyqhx.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gaenikavv.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/govgyikgl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gjwlilgsq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/grvolfzwq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/guyfjqslm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gazmfiyqy.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gfvhiigvg.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gynybcsya.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gbsedykum.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gjynpisrv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gtxzthcuo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gbsaasgat.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gwjihezlb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/glybnkkhv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gggdzsgfe.sHtML


<!-- 参考信息 -->