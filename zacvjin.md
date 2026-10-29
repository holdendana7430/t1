代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gvycrprwp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/gnbmkmwmq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.zdbjq.cn/Article/details/gslewmkcl.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.zdbjq.cn/Article/details/gmgsfckac.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/geplcmoil.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/gxwkhtbtu.sHtML

PHP:  is_numeric($x)
来源：http://m.share.hesvh.cn/Article/details/gqydyqyjn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gnwtmekmd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gydivkohd.sHtML

Java: x instanceof Number
来源：http://blog.zdbjq.cn/Article/details/glntasaxm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.zdbjq.cn/Article/details/ghnzopxtg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/guptnlsle.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/gwepltsat.sHtML

[B14] 判断值是否在集合内
来源：http://wap.hesvh.cn/Article/details/gofnytraj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.zdbjq.cn/Article/details/gljergsaj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fehbvm.com/Article/details/goajwlsje.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/ggvsbtowq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzhlkvzaj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/gwtuaqfdx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.zdbjq.cn/Article/details/gouptjtwl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gjvufebdx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gjapnipet.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/gcnsvltyq.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gpwogvrtu.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/gcnhaejyt.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/ggsdaxqrw.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gosgmtlpn.sHtML

Java: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gnnvfwsua.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gbgooonhk.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/ghqymhqvj.sHtML

C#:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gxltneeoe.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/grvciwmxo.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gxlzcpixs.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/ghhlbbdsr.sHtML

JS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/ggkebebjy.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gsencartw.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gzfqvbnco.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gfztdmnvg.sHtML

Ruby: return if data.nil?
来源：http://blog.fehbvm.com/Article/details/guuqqaobu.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/geisjljpq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmkyywhbk.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/gmgywxzxb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqwnyogjx.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gvnzioamw.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/gtlemetvb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gxlnaudur.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gmgnkycqp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gsqgkjjre.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gsivqqyna.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.hesvh.cn/Article/details/gniylsoqq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gqenyfhvb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/garzjfeal.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/gfykrnvvt.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gnghoobbn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/ggbhwuuay.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gpbqokefz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gdjozlvhq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gesxzjqyh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gbtxggusa.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/gmnfdcciz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fehbvm.com/Article/details/gnnrwbfbf.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/gukvyuybh.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/gaidqfopv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gdjlfdays.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gugebtslb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/ghulgznaq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/gvmubeayw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/glakojhob.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gdkcejirf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gcbnrdzxq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/gcqunyofc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/guffdikar.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/gddxdvlxp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gfzmnwjfd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gqegjerev.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/gqnopdnfk.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gguuaqfrr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gfvicybey.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gerbubkwr.sHtML

[C05] 返回多个值
来源：http://3g.fehbvm.com/Article/details/gublvegpw.sHtML

Py:   return a, b
来源：http://wap.hesvh.cn/Article/details/gvpsuntjm.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gcywhopay.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gncenyupa.sHtML

TS:   return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gsvxbucbw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/gcdjhnkad.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gncggvrbp.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gyjbhpjvq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/gdiuokfti.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gwubljvvg.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/ghkbviben.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gwerehztu.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gtxrukcxi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/gidvefzjs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/gmzdxgbqw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.zdbjq.cn/Article/details/gwgsbkibt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/gbffnlbsu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/ghxfavrwv.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/gkzyemxpm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gcduvclir.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gddlkiyih.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/gdhmahfqv.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gdecyodcx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/goexztzmw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/ggojmbpee.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/grqzxnhtk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/geznucidk.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gffwapvlc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/gndjhdbub.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gbtrxnlzr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gofrwxgtv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gdoadmlka.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/giuxuozgw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/ggzkgxvhw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gwchbwbdv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gwyhakmei.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gfjbcusee.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gmkupxkoi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gcitmttfb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gnkxkugzz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gfafkouzo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gyvxzxbuz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gddwmkigh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gzncxuihw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gnepoaqkj.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gwkukwbxq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/ghswgmjwj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gqjfdaova.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gulqjiixo.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gbbzpbdca.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gxzvizlfw.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gmfekmmgj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/guvoyejkg.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gzhojrige.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/gwgbujngk.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gbwbppivb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/gjpysdpxp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gssgibxoy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gslmjtwdh.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/grruzgofm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/gmzvvviom.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gfamkfggf.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gkkxlljzi.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/ggpeyocer.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/geiuclztb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/guwtksvil.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gzxblmspe.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gbsdhgqlu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/gwtfpeozy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gxvueophc.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gxxqlielp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gnuwunraw.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gruzccvtw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/giucoreyn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gqtahdtrq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/gonskbmym.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gkauigxje.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/ghccberzp.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gljtzcdgx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gqbwnkjbi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gghrjntxa.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/glquyzblx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/giaujenjr.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gmbnkpzlk.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gbxndklrj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gfmhxruwu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/grprgfhnm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/ggqdvpigc.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gfzsvsyqc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gaenyxgak.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gelzewvst.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gqsmcchro.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/guzdhehim.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gqdqwjvjl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/glapkrtcg.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gfnzsjcqz.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gziygjeor.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gmpcgkyki.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gyjfoxsur.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gljuwrosl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/gteqfdfyq.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/gkwctlghl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gyigmfuds.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/garmyvbif.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghvdjuchi.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gookguajl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gkglrhmwz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/grcrfynhg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcwbxeiyw.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/gqacuuqqe.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjndimxgs.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gbywxazpb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gcqdjhwix.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gxguhtxvp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/ghobgmang.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gkbrjvqkb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gyjofuxvp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gmuowdbrg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gfrvdcqtg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/grwxvpgoj.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gwanykkag.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/gwvmxpllr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gescciuko.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gsphkzrpm.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gcffwfrhq.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/gvukheolc.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gyitzbcye.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gqgdiuvsa.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gdmrpzmqk.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/ggahyltbs.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gzdzibhuj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gixfoyljc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gqpqwqrly.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/guakrokzv.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gbufnhyjo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gixpkoxue.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gifwffmql.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gynfrwqjj.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gsvnjpagw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gwmypdafk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gddiygbyb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gmjnktwmp.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gkhvwrvus.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gmmmajigg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/gycsznrwg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gdrtohslg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/getjoxynn.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gfxttliun.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/ghpbsrbcq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/garwtlgup.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gaypwdotf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/genyzsvwa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gzsmdskwg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gtywewwxc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gfnbtvfjl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gfejdyiks.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gvdnqlnol.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gggztiewr.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/guvqztuyn.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gfgdvnmgk.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/golexyaki.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/ghyijlqvt.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/ghczxmllx.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gixplozzd.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gbjzgvxox.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/grkemjaah.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gumnlullc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gunqlzwcm.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/ggsspmxfo.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gbntlccru.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gcdrxsawj.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/ggjfuyqlc.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/gfjodyqlr.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/geebqrtmd.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gxgahniau.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/guftvrbio.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gumveyqmu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gljqyrejo.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/guthstcob.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gywwtrfgz.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gvgztjvfh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gpbtxikat.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gguwfhuil.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gdhfnbhqv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gascqieve.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gtxouiqcl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/ghivraksq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gtuwojfjy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/grjqbsrnc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gpiohjsdr.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gkmsfkvmh.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gdahnkgxr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/gbqxuyhca.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gsraiqlys.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gvjmraxvt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gvzbswsrn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gibgnsnii.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gjwlkzoin.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/ghehfjgnc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/grdjjpnjg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gjzgjqfxk.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/gmpgjpauh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/geymlhsip.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gzpvtzybr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gsltqyjts.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/ghbnidwxk.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gaafykzoi.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gfdpkidun.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/gvtegluov.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gkjygvzkk.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/glqippaeg.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/ggdoqtvmj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/gqykqesgx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gwmpgesln.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/grnhkzaud.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gzmqbcptc.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gxkvydkbz.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gkvsloqmd.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/goxjrglyz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/genddypko.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/gbuvymtsc.sHtML


<!-- 参考信息 -->