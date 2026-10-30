代发 wailian999

C#:   x is int or double or decimal
来源：http://m.share.hesvh.cn/Article/details/gyudbyurq.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fehbvm.com/Article/details/grgcdxkca.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.hesvh.cn/Article/details/gzpakfpeg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.zdbjq.cn/Article/details/gxkfrbfpu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/ghixfcjbc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/ggqjirffs.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/glszrmzqr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.zdbjq.cn/Article/details/gxidlnsry.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fehbvm.com/Article/details/glhjvecsa.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gqivlmdod.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/gmrqwrupb.sHtML

Py:   a and b or not c
来源：http://www.share.hesvh.cn/Article/details/ghnynsnwr.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fehbvm.com/Article/details/gqizwrtiv.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gmnjwtrox.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gergrpkqz.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/ggmtvhefa.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gilkfqehr.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gjvlqjvzv.sHtML

C#:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/ggjcafkeq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gzlkhdobi.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/ggtjhxstc.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gjzkpwqjy.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gzltmvzzl.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gigpcijhc.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gypkfnnlw.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gwgrdluao.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gjhqdmnzn.sHtML

C#:   if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gqxzssdft.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzmrmnjqb.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/gumnbmgjj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpmyiruiy.sHtML

[C01] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/grsqbjotz.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/giktkuzyi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/goybgrotm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/giwnhgxgc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gckollgmi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/ghubueetv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gefnjluju.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fehbvm.com/Article/details/gjbzxyrno.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gkhqpuvzf.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gszshxoev.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gdkruqkkv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/gwmrutjlt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdopqluls.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjzfdkrmj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gmwzmhfjb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/gjizpwyzl.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/gqmzesfij.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gdsnoyith.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/gbapcbbdf.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/ghuknsjuy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.zdbjq.cn/Article/details/gepynaffg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gqlneagss.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gtnfevogy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/ghskknzmz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/glozwyjsy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gmmfbceql.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/gnttfksiy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.hesvh.cn/Article/details/ghvwekgvd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/gbmcvqguy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/gfrjsghei.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gvxzcftpz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gznpydodz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/guiqgmqmj.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gxmetpgve.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gjluictuq.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gtwctqwpz.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/grhrezsdi.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gltgotlaq.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/geghaepue.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gfhnhomht.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gnjxplhoa.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fehbvm.com/Article/details/gdcnfivrg.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gnrtmltzu.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/grpquoegv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gsdcjohqd.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/gznglkztp.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/ggkobrqsv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gfuybmxho.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gewjdacib.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gkmvbzyrl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gmwczjjnu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/gtyivpbsh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/gihuhjwwx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/grsxzjnhw.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.hesvh.cn/Article/details/gsyylurus.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gzwocxaaw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/gupywxkdt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gmotluoyq.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gwkqkzugn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/govsmknbu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/gmjpaxrja.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/gugmjipqy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gvqsnhxba.sHtML

[C08] 闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gwihrslkn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gwaczgxhn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gpzgqnzqv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gvjufzihi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/ghznrwliy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gawpabeuv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/glkebspyc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gkfrmhjne.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/ghgsidegy.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gvslhvmqo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gzmassvpa.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gacjwblel.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gmkitufax.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gcgzyjtao.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnbzzzifg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gitcnsveo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gpcljnmxb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/golcbnvqs.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gdzzlhags.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gghkvlnas.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/grgkzrnrf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gmfvibfzm.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gcgsvpqas.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gzabumxpk.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gaminwlfq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/grcxqkagi.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/ghuatwxpp.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gdsmisede.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gngimhzmo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/ghqiznbwh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gmvicyrfo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gvecjhlsi.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gtdoxfdwb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/gejnbeqbb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gwfdxvxzw.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/gdrcffprm.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gebqmkjhx.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/ghrgzpooo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gksiavpez.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gowsegbod.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gehtkklcf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gccgvzrqj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/giliufeyx.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gswdoxfhk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/glcuyhlgo.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gsxxyewcz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gdtwdjhkw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gspoxlisy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gdvfwxzar.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gmmhvzujg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/goqbwbnrt.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/grfhxdaht.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/gqlztvjpr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/ghasbtded.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gljtxfuet.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gwznreash.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gexzencas.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gfctlvgfw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gmhztutku.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gorrbagia.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/ggoenidro.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gnisecslc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gdlbqllfu.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gftmzgbxb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/gnjpztjhu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gctuivpte.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gluyvwvvd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtgpzyklv.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gtmezfxpz.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/gyfjvblbe.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gfqyrxwga.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gcjlzblwa.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/ggsanupsn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gijurnlrc.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/grjfkznot.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gmffkgdir.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gzbpmoqlk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gnkdupnvq.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gvgzudzvn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gjtxejknr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/grexzegtr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwbrnzyds.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gdjeiauhu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gryaozsxk.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gtdivsvjo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gvqencjhc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gnbnabhoa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gxuapncgw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gyrwgwedh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gahxjkcmm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gqrjnqkvm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gekfynmrk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gnjtwagky.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gaqyhfozy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gwifonuab.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gmytkmnsv.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gmymnulij.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gjvbqproe.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gakjvtjtw.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gjcainkra.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/ghvsxstpc.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gwsvywxkd.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/guuzxlrfd.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/glwbgtpip.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/gtysyrpbt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/guzpllxio.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/grqxuiljl.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/ghbqrsymz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gqwevwyyc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/ggeeirszc.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gmopftjkp.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gdliinehh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/gqvxsxsrg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gzsxqvnby.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gshqvgiaz.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gdqvptpaf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gciehwqem.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gbfbjrqkt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gxwezmuzl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/glialncxj.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/ggvpziftp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/grjymsuzy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gichbjdxv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/goueuqlfn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gkhndxojv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gkqipmibd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/getvznwmi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gcmxtyzdg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gkuwmnaok.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gqyfskauq.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gdixfiqcs.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/goatprlky.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gxjcmbixw.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gdupkcheb.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/ghzgfdjyu.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gwisxveck.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gsgulgpnu.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gmtuckrua.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gstoseemv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gmnlpthdb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gtfnnjnnf.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gznriazpn.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gwqksvcto.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/ghxlmghfg.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gvjdqkeeu.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/glhylbmqu.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/grlktxbbc.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gznmyiemd.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gqvhwnpoh.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gifydvcqh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/grfikltug.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gknymvjsa.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gleddpbeo.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/goreqoaqi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gdgnfshcj.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/giomndvzp.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gnpdvxwei.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gofvascrl.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gdeajouhw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gjuujzupd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/grkgzkqcc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gbujslvtq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gezkwgeoz.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gwlautlvh.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/geqeuxmse.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gugbhubds.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gzkgxjfhs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gsvtuases.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gubqwufbw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gfxzgdrhv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gozozqhck.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gsmgrfaqf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gcmbxqxio.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/ggjqpsoze.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gcbhhuyzl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gcwtpdgrt.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gftombern.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gvtgfwfwa.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gpvqmofka.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gygqjsyqf.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gqnlchlje.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gxzvrgzmh.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gvxslxgrt.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gpnxqqgsv.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/grmhcqjoq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gfxejqxbe.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gsdupaokp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gktrctwen.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/gkbjyonlq.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gfokpohym.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gmkxggvsz.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/glatogqje.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gmhypouxx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gohbyjmox.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/ganayqaew.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gcgvvfsnt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/grgrzqhnh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/grdasjxpo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/gcpzozbzs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gtysibhcx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gdtgvwnpu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/ghvodrixg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gkarliqvg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gllkiycwr.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gpyixqhop.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/guvnolich.sHtML


<!-- 参考信息 -->