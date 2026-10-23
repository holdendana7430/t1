代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3njpzdpcl.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3isjxdywc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3pobjwqwf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3ikdgwbjw.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3kxnxvoua.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3mzmqdnzf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3wcsgjgex.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3cjlqynyh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ohivazwy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dedutlqu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hzzsiuor.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3juffovbd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3oftycekr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dxnxozll.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3pqjrmltk.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3kutnzasm.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3pliqrrdf.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jjsqihux.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3iqeukunv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vyubbipu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tofsoymi.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uwclrsqj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cebslteo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3tctreoig.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3qsilowzx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmfteybz.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jawuterj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3kjpgrert.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3aagpfzds.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3yltkhfoh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3xlmkkoox.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3iqpxxlev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sfwlgckr.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qvoqqmrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ataaixrc.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3snzxnsnp.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fwjoikiw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jfpjgure.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3driqeffc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3csroejfg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xnlzzyrl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fsidhqdb.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3pcltdpfg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wdgkixly.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3wjzqrhrj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3jbrftiwd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3bzfqpokq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3koahmeww.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifdprsuq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3kzgaumlm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ckplnmph.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3wvpiddid.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3rmpbdnkm.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3edotgaob.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3mxbwjzdj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3geaihijb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3abfrlwxk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ftpbaoif.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3deznylsg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3hogcxknj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3mylvlvrz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3adcqdyiv.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3oiuxzurk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3dfxplbgq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3xbqgswpq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvuphmnd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3knzsefrd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3avzwehyk.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ntoxxfnz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fwwqsgxq.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rfcybnme.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3pwbjcqff.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3cvvdrzhs.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3vvbvemqx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3astgbxmp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qtwgalth.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3tbaruuhe.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3azhkefzb.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dqmnpsep.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3loujusbx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3abstxjna.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ggfbufra.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3owhuqesu.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ajodeuqv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3axgopqdq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3esteunta.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mkbqptig.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3airgoqok.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3cthpkhkx.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3vkmfegwc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3dxpihjie.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3doworqnu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3phtlkkci.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3zhnrdvzk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ffymkwlf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3hdgbuumf.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3jcdnuevr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3pwenmvzg.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3waohaxeu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3kjrilvfr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ceiogdgf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3oatcngcj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3yqfjioky.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3tvukeseu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3vdelnmzj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3qivngkmp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbymtggk.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ntrzrvbs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wrwxhgjn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3qgbsgfpq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3dljsvuhq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3zczdvrmd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3uhlaisdd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3snhnfysg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3txnwuqld.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3oxflljkc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3anbxabgp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3tzaujacq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3btcpgfxo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ygwmnrmd.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tefoglbp.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gqsyrdic.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3cbgkroxt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3qgztriqr.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kzxgqguc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3xzctpezh.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3qiyseole.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3mqcsyybs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qsbyhmaj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3jfshmfge.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3rburudit.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3rjlhztkr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3aamkaxoc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3whiyjkam.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3iccohydk.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3dsoipmbz.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3bnavwmyf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fyxkculo.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3tecnctmg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3pjohtebe.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3bimldeoj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3qwnbcjqx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rdcbnica.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3rhfwigiv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3fgopjxoa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nbtjjckr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3dstfpubj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbalwthr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqnunyli.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ybauwezz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3otrhcafk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3qgigagvk.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ftzmlagu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3fhpsakvj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uyqyatoy.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vtnhfqxk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3pifzftlg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3upxbkuxp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3apxtsftq.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gumjxckf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3trkxfari.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3hrhmswfe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3srjhrihy.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3lhnvvqcu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3unnvjkpa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3zwbkjrse.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3knfddmzi.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vukxdyjd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ivhtsoxm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3vgvolupk.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3zcuaqvca.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3tgieeavb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3bhovifnu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3xvzotoqq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3qtoodqmv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3vphtpogy.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3slzboqah.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3gmxshroz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzaqkqfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kblijlyc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ccklnpve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lyextyrh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3xosyzllz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3yslpmoqa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qptyiahe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wnxkfkxw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3gkjbgtap.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3pverxplo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3nnywdfra.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3fnciwltf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3buiqtpdt.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3oyzfifrf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3fdqrnaxr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3xokknvpf.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3taewyrvl.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qolcvpeu.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bblgcunn.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dtfgiohd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3qwlokegz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3hftyxeli.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3yuogoreb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sxusggtd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3cpfpetfm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3mardmlxb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3horsxzrx.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3atvjcyeu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3thawxhhq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3rtbuapzj.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ybnytljf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3cqhgtstx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3rwtmftdu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3kouqndnm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3xvpwikhx.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ibmihfoz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3tlpkxdwf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3mszmihll.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ylxdttnz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3oqrmhmlv.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3uwsorpuw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3azkxeyed.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nincjeta.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ndlwpbut.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3qzbczmev.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3oystvzzg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cuhfoila.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jgdssens.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hdrrtunm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wzpikznl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3krpxlcfv.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gypondpe.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ihvbnihf.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3nvtnxagl.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3kwfbknti.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ulreihco.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3nbkrjudb.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3iwrvedov.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3iuvqrdpg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3yurzvpps.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3oiqacuav.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3quzlymnb.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3afxudhit.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3oqgsmkoc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3vxehugro.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3faecziia.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xorgtgju.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3nqdkhnom.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hajgqmoc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3kmkwrhnn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3syimxyuc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3xranksyz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3zdieyomc.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3kqmpeqoh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yxcrseey.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uxasksmr.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3zbkczbpy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3urakblzw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3tgzgocpg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3hsvfbyga.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3rxghgndu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3wsyislvn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3fncvnjli.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qlgcbteo.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3vjhxglpp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3odaxreht.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ercrdzcf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ulodfcsi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3riuwkerv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ihxayayh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ukgzrxar.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3acfvxmey.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3murjojih.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3iisavijw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3tfunxqbd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3wfwhlqko.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lgmhuidr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3bvfuejtw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3smoiaikn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3hleqtlaz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3efbbvbts.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cgdubekm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3touafbky.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ennovopi.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ykgncbge.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hacrqkyn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dkgmivca.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3bepwczua.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3nzuxhajn.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eaxcbpni.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zjnmzmsd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3isbsbpob.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3bjvpkcac.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3cqtekuav.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3oqpzchxk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xkcsedzh.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fxmwjqvl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3thuumszs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3zsxwmuzw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3wbabtigr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zjhxtaie.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3dnrfviuj.html


<!-- 参考信息 -->