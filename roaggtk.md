代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gutgbfzdj.sHtML

Java: x instanceof Number
来源：http://mobile.fehbvm.com/Article/details/govznhuka.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fehbvm.com/Article/details/gtirgbymi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/gjgpjwkxy.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fehbvm.com/Article/details/gemldmnku.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/gyjoicciv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.hesvh.cn/Article/details/gyhetyesf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/gwhusbmeg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gsvlnuxhj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gjazfxrxe.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/grvimyxfn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.hesvh.cn/Article/details/ggqsvdilq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gxwgnkmzs.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/guzczjkhy.sHtML

[B15] 布尔运算与取反
来源：http://mobile.hesvh.cn/Article/details/gmdnekrec.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/glhleoses.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/ghgviznsq.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gwizmqaoo.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gagoxgfkk.sHtML

Java: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gxqfxowzr.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gcijkxqlr.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/grrldsqfa.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gzgdvxzgc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.hesvh.cn/Article/details/gmlucaliq.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gmsplsnjb.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/gzcymahfl.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gyodfmecc.sHtML

TS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/goneufpiu.sHtML

Java: if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gtixcgekl.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/gskmdntht.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gcqxiprxi.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gtjdxvyns.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfvzfgyho.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/glcivzqbe.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grzsvvwqx.sHtML

[C01] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gkgkhxweu.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gwlvockio.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gsopsjzoz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gkusnhjrs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/glymhnogs.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gaeaksjas.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.hesvh.cn/Article/details/gumdvoxuu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gbneydkfv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gspojqrpv.sHtML

[C02] 默认参数
来源：http://read.share.zdbjq.cn/Article/details/gxhgvbgxh.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gbebnffku.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/grjibqjgm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/grzzrhgoj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gknusvyrl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/gtsjcyueu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/ghxzblgrz.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/ghduixbjz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gxchwxkeu.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gshbyuhvy.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.hesvh.cn/Article/details/ggxldbihw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/gsoljkhiu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gcltkkzzx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gllcitpdc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/groivxaoz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/ggqpfqtjz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/guymphxsn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gbwmighqy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fehbvm.com/Article/details/ggjhaiwjf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fehbvm.com/Article/details/gtvtbxhdo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/gkcztiuag.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gfnbfcxzc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/gzckzlwxi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gmyssptfl.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/gejegfoul.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gfyvxcqlg.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gbqcxszsd.sHtML

[C05] 返回多个值
来源：http://3g.fehbvm.com/Article/details/gsszvayxk.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gdalipnuh.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/garmrnqls.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gfzkfutaf.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gbryhavtn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/gzpgwqpdz.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gixehjcif.sHtML

Ruby: return a, b
来源：http://www.blog.fehbvm.com/Article/details/gyjygcxlh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gigphcoxj.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/gkvemvqgs.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gzvkdchtq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/ggytrkrdd.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gjzgbvsdp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gixjjmgla.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/gdcfchsuv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gfntidyds.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gdjvrmyfo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gzziimata.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/gfnomsxla.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/guwaisazz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gyvjdhons.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gepldictj.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/gehueqesf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/ggprsjycf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/gufprwinw.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/gqcbmzctw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/goeisonwb.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/glpyebgwl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/ghyvrcxqb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvquppeer.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gcqlcprko.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gisyysfjg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gvcmdihen.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gixwpajkd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gyoiqlnsv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gcweeplba.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gefdksrcl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gjiszatbc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gycsdnsgu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gsmfbpzud.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gejisiwrw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gjvkewson.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gaciwedxi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gwddkdoze.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gmbpqhzox.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gmrgvjcdx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gkjxqoity.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gcsmfkuyh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.hesvh.cn/Article/details/ggklswloe.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gjpxczlgh.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/grvemsfyf.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/ghetzeizf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gqgcszkrg.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/guxqjirgi.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gglvetdfm.sHtML

Py:   from module import func
来源：http://www.share.fehbvm.com/Article/details/guldopxbb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.hesvh.cn/Article/details/gllfqgknj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gpvjoxrvk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/grnouuadj.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/gcuvcbyfb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gbaqnnybe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/geohaugyk.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/gksirctcd.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gbyrlanap.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gyrslvlwu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/ggteiitze.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gsyibrsax.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gcpeffizr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gxkzerzxm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gzzyxghpe.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/ghhyhrxrk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/guizlkshb.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gqdrnutjq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gjttvimqn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gkdkulipk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/galxubvzb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/giesofddi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/goggxongo.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gnibogsfy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gxkkrgqrq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gbesyqkub.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gjraupfdw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/glpdufbwk.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gwreneyxh.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gdqhohhty.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gnqtqgumw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gladadphm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gpvucgzue.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gytmstxkb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gsertvumn.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/gcikprcse.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gguhpndgp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/gacnxidwl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/grpjmhirr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gbdlxxtbk.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gpabruvxj.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gfpczqwjp.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gqzejuvjx.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gldpgwkxg.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gupdhdtid.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gasoruehm.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/gqqqosnwu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gszeybptm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/ghrozmqcm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gahnuasyz.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/gxtkuvxps.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gtamnjkyu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/gqxvheigy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjjmsoijh.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/guyofoahn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfhqzwqpa.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gvvicqxod.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gzpwxxwam.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/giukscqzw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/gpiuczlvd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gwhsxyufn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/gfqirfilx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gfvxujjpa.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/grdksvzwa.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gyehyswvu.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gvzxrsexg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gutheljar.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/gmtekulfd.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gvugzjdio.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/grbkxwfjf.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gqmxrwine.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/gljpqbkln.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gffxilylb.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/ggrvzsvnq.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/giddtpluf.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/giwpxyufl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gxdnulumn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gtzivfujk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gwsyinhcc.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gzdgterxj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/gbswadtxb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gtiluizlj.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gcdcwyqpj.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/grshayakq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gfsvxqjlt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/ggxjyeqfi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gucdjcpos.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gmpwsxbzx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gvacbjcaq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/glcbhlbjq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/grutltvju.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gsudmkqdr.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gojbzqgya.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/guukjmxfm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gpluauzhp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gcdahljpw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gfsjislev.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gakibystx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gmbnatzjr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/grbwubyuh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gxkosunqv.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/grxsxskel.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gzvgiumwh.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gtlmbpknc.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gmzduazay.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gcgtqgkux.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/gjxrngubs.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/goejwykoy.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gehfljjxo.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/griivvzyd.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gcmkobogb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gwqnkynzw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gbuxotelg.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/ggxrrajmd.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gdulaiqpn.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/grpzzteci.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gquuhzupa.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gdpbnkzek.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gjgodvuzl.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/ghnbioldu.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gahugfkhq.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gymrlzaja.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gpiaqrjtf.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gqqwtitqp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/goktrgljz.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/giacocxvj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gobyoixdd.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gotouhqwk.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gvlhpncuw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gyjrmgzaz.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gnnogbmox.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gauyhswns.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gryfmwgjx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/ggigpsngp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gcwlnxyah.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gjwancjga.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gzyxttgca.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gyrdhjooc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gcalvaczw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/glhsqkmmp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/grrwlefif.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gsgbedsvj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gxbyfqsrt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gozvesajl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/giaqbrpfo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/ghcascbyx.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gkptibkis.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gjqxqfufl.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gjlzbmfdv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gnvvfoyxh.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/ghiavtzhm.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gjdwfqvyd.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gdfkvkpqh.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gaiedfyll.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/grubmokms.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gbcspjmhe.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gvgzglxjx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gauksbhez.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gmzrxnypo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gfvlsjarb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/golywnbpf.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/grzkodrsl.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gdkhivhth.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gqouthbap.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/ggmyowbem.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/giljkgxsk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gvlmgxdqr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gesdzvgqw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gxksjkcmi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gjirtwzdh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gjqssxzcx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gjtjlbwel.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gqghrrkyy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gulbcsqxh.sHtML


<!-- 参考信息 -->