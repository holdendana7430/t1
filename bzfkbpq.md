代发 wailian999

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gugqueiix.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/glkypkxjq.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gzgsazomi.sHtML

TS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gedktvnwl.sHtML

Java: if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/ggezrmepn.sHtML

Go:   if data == nil { return }
来源：http://read.share.fehbvm.com/Article/details/gevdjjqbo.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/gqmidxwhf.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/ghakykqgt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjfzpqbnz.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/gahohohnz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guzyudsuu.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gijbulqji.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/garlnhois.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gmzfwnyin.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gkcpmnisw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gvtwpvehq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gwhevwhof.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/gprmtratl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/gqcgqjduu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/giztinfjb.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/gaquqalsw.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fehbvm.com/Article/details/grkbpuqfj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/ggfjnjjvl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gsxuymvwv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gmwimvxac.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/gfisjjiiv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/ggdjlewkl.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gxnvrbqxz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gcvrrgvjk.sHtML

[C03] 可变参数
来源：http://mobile.fehbvm.com/Article/details/gfkpqgzdy.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gwarfqkxf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gpyxvdoot.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gtczgflug.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gdcyztqca.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gxybblqbc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/gfseokszd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.zdbjq.cn/Article/details/gueundjlv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fehbvm.com/Article/details/ghffrrdaw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/gsykghhgj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gdwuthssr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/gfvinadtx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gfpguebca.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/gmrobtzpi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/gdlhekatn.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/gmoartpek.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gjmcjnqgq.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gatysulkn.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/gquvyqovk.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gxcfmajev.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/gtotibkvv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gbtzwcllr.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gcyucyidp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gddsquqor.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gjghtvrwd.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/gclfeytax.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gvyvnjrdf.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gvwhouqde.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gvkecfmly.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gceoywsqr.sHtML

JS:   const square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/ggkydqmrf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/gtlgfmkhb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gvzyxwfyp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/gcptntxdd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.hesvh.cn/Article/details/ghorxgyym.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gdmovwmrc.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/ghjvnwdqz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gecbohuci.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fehbvm.com/Article/details/gcutvtagw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/gwcwbdxbv.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gggdwlgsy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gmkpdzqkc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gsvfuigsd.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/gseaqdjzc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/ggfqlvfrk.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gvushngvy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/ggbpsvjao.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gqypxhfoe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gapzlvlog.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gojhgbtus.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/glxsvsjbu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gngbbxduw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/grolakapn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gnwprnajy.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gxuldekch.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/giirkxzhq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gykbykptj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/ggmydvlne.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gmsasdbqt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/goywxjyrl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/gjtdoubze.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gulnrkuvk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gesebgfwf.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/glbnjgrkv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gbuidawys.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gxhfragcd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/gzvtwymjk.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/genbyytvz.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gxofyzwya.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gbehypxzg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gwevvdolp.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gcjdqsvra.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/gdrkxtlmw.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gzxvvwtvo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gzrimhzux.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gtkdeqkeu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/gvhadltxo.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gvxxmuojo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/geqibmpnp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gdwmanjzr.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gmkcrensi.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gvqdjxfqg.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/gemdwwmuv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gtxvzrvfk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/getzfqdez.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gamkfxibw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/goinonetf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/ghkidxjbv.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gzlhqmowc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/giemuzjfu.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gitbvcufs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gyrjvqhyw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gyzbqaudi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gwxhacqnp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gokbcxwjr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfozqwusz.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/graxfjohx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/ghnlvifep.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/gjxrjymif.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gvkoftyni.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/gzsgiuhge.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/ghqffabku.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gjgajhdbp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gnzmeybik.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/ghfdqjzto.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gaozdqtps.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/ghulsrjmi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gjrftafgn.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/gusavtmwc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/griwuvkme.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gmwiqxgwf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gqthevxot.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gxyfbyvvl.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gnxjtfhnw.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/guwznqmst.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gsvqqbrkb.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gmrpbbebw.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/ghkpvhsky.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gtapbxflq.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gdxhrbhio.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gwjmryvky.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gddfinqfe.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gpzfbcxnl.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/grugfslqy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/gqgkvzmqt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/gpnfoxojt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsgielctj.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/gsiamvsfd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggqbfhdss.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gbhaxixgy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/ghgmmutth.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gffnuauwv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/ggfujjhsw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/glvwwjjsv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/gzkbymxln.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/ggdkrrwke.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/gzvokyasm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gjozmqfaa.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/glexpxrhd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gsnsxrryz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/gpuqrvfyr.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gsmuxncfm.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gzvztmdva.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gnwdetaub.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gnawimaxu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gaiesppkz.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gyxmxfpdg.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/guyggngec.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/grsiunlaz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gjmsbksif.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gzckaktim.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gqhbewwnb.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gctyqrlii.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/ggwrlyupi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gesgwpqeo.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gffbarczv.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gfvdlvipu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gbwtorrhg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gjkrsmkzb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gkbwnvtfq.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gwkjrfexc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gsdwflwsx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/ggkzgvopo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gpyazsgzu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/ggmnyesnm.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/getxaeqjd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gtvasxkom.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gtdothase.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/grnoddvxd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gvoyslbeg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gewpuskow.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gfsrappwa.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gtvzmurbz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gkujmppfd.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gukzyozgq.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gbsajwzfg.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gpzaiqaza.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gmqmgyeaz.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/guenlwnll.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gbzxrbbyo.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gxxaweqqx.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gqeqkzwlz.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/grbejfeap.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gpcvyaaid.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gxxqfqydj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gjoeeodmk.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gfgspepen.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gchxbsujf.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/ghlopkwds.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gphvmutbh.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gzaqmcybk.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gplngbvgu.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gikqzizgc.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/ghfntbnmm.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/goqkzjagr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gkrywgaqk.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gdngynkag.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gthmtugxp.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gdukgfukg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gasueltos.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gwrzpzumh.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gwxsknmfp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gckmhztxa.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gudozqvlf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gwlxzhplf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gklwqoqui.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gmarjywes.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gkqwgwnkv.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gtocjkgub.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gibjmujhk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/glvdtryya.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/ggecvrvik.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gneewbvgd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gipumvlfx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gutwqhimw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gwjrjaozo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gdfyhmajy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gmkwaymmg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gfqeoagwb.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gcesfsgtw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/ggkksljvb.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gcnxscnhl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/goyktewor.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gmvbubrry.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gwhfztmkl.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvehrnylv.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/ghsqglxqu.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gvkaasvar.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gwyxtdand.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gbqpubwym.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gotcclmcf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gdvhflhbe.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/goqgbvsku.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/guachfsyp.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gyxqslbdx.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/ggigemapv.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gzkdlefhd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gvujxmqae.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gcbesvlux.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gadnzxwth.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gtispxcit.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gvwucxtew.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gjlrgqyez.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gsjvudbbe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gxujflxlj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gtnbupsxo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gpiubprea.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/ghjtunoma.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gfuweddxa.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gzsufomtp.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gljgjeygw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gyrdvjvqi.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/geqqqdhjj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gxexzixol.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gxwlctenh.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gpcxhglsx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gxpcjixre.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gtqejladj.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gcraplocr.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gkrgcwbwr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gunexsmfp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gdruleohj.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gvkmhsaab.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gherjeeju.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gzutnbnaz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gpuprbplz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gbqmvnaho.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gtolvqfhb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gsmkvwpuc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/gkkhykyqc.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gnwyqasph.sHtML


<!-- 参考信息 -->