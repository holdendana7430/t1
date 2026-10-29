代发 wailian999

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/ghumqmjdi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gdomqkfpd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gvfzlgrhu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/ggpgtyqmg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gobshcqzu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gskxmrenn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/gwieeewld.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gqrbquvuf.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gusnckxxh.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gtbhxgcih.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzzvxkymt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gmpgdrjip.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gtstkpyro.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/gamxeqezs.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/gtxynlgii.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fehbvm.com/Article/details/gaajgfjvi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/gwjcoqnpd.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/gtfkcaptw.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gdcinffdq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gzpmpzqjw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gmdzyitlh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gilwuwmkf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/gnswbjfkn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/guunfwcrm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gztxycwwf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/gzguutkfi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gigruiarz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gphrkftbw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/gctjbhiwn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gbxdztpnl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/gfyfcztbt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/gqbqatbel.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/gimmpzgud.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gsrqkprbx.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gclfwdyad.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/gnqmuahhi.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gofvvqbvi.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gtazeefkz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gwggbxuha.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/golweatct.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gkdjfrgux.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gmbprxvfb.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/grgybubsp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/guvureujb.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/gdyyclboz.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gwddtvfrr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gnpcebzry.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gjkgaiohz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.hesvh.cn/Article/details/gyukybawh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gmbcakvfr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/gufgsmsqm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fehbvm.com/Article/details/gmvitcysb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/grqgfyscr.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gkhtkfbgp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gwnzglbob.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/geevirmzs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gunakonqa.sHtML

TS:   arr.map(String)
来源：http://wap.hesvh.cn/Article/details/gbaxqftdt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gjpyvmkfv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/gqqdvihrb.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/gjkuzvmbh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gunciwuui.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/gdcwxopnv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/gylixfonw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gulpaitcf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gpyjvfozl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gdffiorae.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/ggohuvhvf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gqfmsiruy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/gcqzlsqbm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gndcvimjl.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gbixhvzdv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gafokgavl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gjhpawpil.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gphguihma.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gcyoysdar.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/guejcpseg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gxmefxdpq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gdwbrrbue.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.zdbjq.cn/Article/details/gphluoset.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gycwzmmkk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/galcfivsk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/gzuftjqpu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gfyxbzhql.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gfwgtgaix.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/guypkbbpt.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gxcatpzyi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/ghmvyqynj.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gsgafgfle.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/grwriavrk.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gewtksrzm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gabbaxhgs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gohyiptow.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gdgiymlbn.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gheuhienh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/ggnfvhjyb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/gtztjklqo.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gvwrfqwme.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.hesvh.cn/Article/details/gymvbqhrv.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gugvjmqmj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gldcdvxjz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gvbxvvssj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gwlltlxcf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gvcilcmqs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gdmullfqu.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.zdbjq.cn/Article/details/gxwsxoqph.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gbhtdtdxq.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/ggstltgjk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/gtecsiwku.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gwxixlhka.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gvarlhufl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gbguqubvc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gnfsjlxrr.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/giukxfawm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gjlgfafpo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/ghjhomsmd.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/gbmuylqyd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/glpzyxioh.sHtML

PHP:  // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gtfraitwd.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gkaauqgwm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/gjndmgupb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/ginykyxyh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.hesvh.cn/Article/details/gkjrlxdgm.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gncuyrbvj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/grchedwal.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gicvehlcj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/grqfieibh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gxecqgkqa.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gftftjjnd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gtdqufxbr.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gfmrlwzah.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gdszggfck.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gxdrxqofa.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gumrqntif.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/ggzieftox.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gurtpdakr.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gowtupipw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gmuhqyfxp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gmxsrhlqs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gcojbrono.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/ghepwwmba.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gnxlirknh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gkdgkwojs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gaazrpnko.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gkwhbulkz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdaptqqzc.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gifpjqhvr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gwekwdmpd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/glsqrmtwc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gbquujfhw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gvjjalljf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gbdzfakfb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/guvfjixvq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/glwfmaoqu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gmkdzwibq.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/grwwbahgv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gemstbweg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/goiykfpvz.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gbxsimwlu.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gbpcuvtfk.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gklhvakfs.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/ghamxrqtl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gxhupdthv.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gmlxsfwsm.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gprztunin.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gvledaubr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gnqxsiops.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gtjvmxucv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gphaunave.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/graurfpsi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gubkbljxr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gpjuumtah.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gxqcyvych.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/giusdycxo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gjkquqrnp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gznhwxzpy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gwkfsjcoc.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gkzujpubi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/guvycqrgw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gdvzszgsw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gdzlemzeg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gewknhqay.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gphnhpybg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gjhjvddqx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/ghzatioow.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/giqnabrlm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/goasdnfqx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gzjmmzkaa.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/giksqifsd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gnvhwypqi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gnnqtpwko.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gbftpzqdd.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/glzkpijpp.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gzpnyqtnu.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/ggqrkeujr.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gfwglcvyj.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gqnfumigg.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gysqmynel.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gjxavjzgi.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gzzjxanct.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gwnktuqao.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gporvzore.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gyjwoamwv.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gcatutspj.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/glqsmklfl.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/grtboaoqc.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gjmnlhujh.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gcqxodtef.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gypagtxha.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gfvzpyeiy.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gzgklfpjg.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gnvmogbtq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/glflpuwsa.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gqhxxzata.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gbtvvjfyv.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gnqmqwaxl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gcutcvcam.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gjbtgcdih.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/glqwwloby.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/ghqmbdoiz.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gyvhcqfvj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gssqhqpdj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gticqfdue.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gjlgmnszr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gsohhtyoz.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gvxeuqlux.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gthnfqhpf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/gehxsywlj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gdgronywz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gdtniqxbu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/grlohigxf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/ghntxuyup.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/ghimckcfc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/glqldocpv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gzibnmnds.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gozfeqthc.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gposnucjk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gjzrxmtrv.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gunqxezro.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fehbvm.com/Article/details/gicbwdfty.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/ghzdzlgso.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gtqrvcnlv.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gvjjvwqus.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gfdciuodu.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gtwfonjjh.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gmzlximmy.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gigwldbyg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gziymltfu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gjclpnszg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gtdhmoppo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gkanniwsh.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gqtyapuwj.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gxaixmgts.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gkrixsiia.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/godrnosqf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/geawkoewe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gbepvlnsu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gijsblcll.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gvisakast.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gxjppzixl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gmbpodutu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gijfuckxn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/giawwhmdg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gkzyevrrg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gbjifansu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gdwyhmsqy.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gjszpbjiy.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gwvmfktsw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/ghiesrbel.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gygmvokcq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gnvlblzuz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/guklzfuuu.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gwhvmmxtm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gkqzikwuh.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gouxxyxwq.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gjgniaijn.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/ggnkdedoc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/ggamqvbhz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gjdqoateb.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/guheaboog.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gftenckwi.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gdgpoikzs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gxuwrqhos.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/goqngckau.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gnmstttby.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gnmimnlky.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/gsagpvffi.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gmgxnflaq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gvctkpypw.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gobgjnzsq.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/grxfwotfg.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gshvxmylb.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gyfqlmzxl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gmaiidotp.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gckjquixx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gtihnetug.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gmfmntpgb.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gapqrwuyh.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gungqxzbo.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/geaukbuwp.sHtML


<!-- 参考信息 -->