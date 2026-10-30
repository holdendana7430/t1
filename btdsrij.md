代发 wailian999

Java: if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gqhiuvjrm.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/gtvkcbral.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/ghjzatwqo.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gadyopzpe.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gitqeaatr.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/gttrjjbnq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtmtxlboj.sHtML

[C01] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gickivovr.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/gnhsfivio.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/giigmeypx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gbcsqrfzk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gsqvudhob.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gqglazbpb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.hesvh.cn/Article/details/glstitfan.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gwjbfbgjm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gqutlxenl.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/gupnmmvfw.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gvhzzzvjp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gwriwtkja.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gfrlgqvza.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gjyzansre.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/gxxjhswmc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gjazgpudr.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/gtdwglmyj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.zdbjq.cn/Article/details/gtpfnqqoq.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gyaxyjcgo.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.zdbjq.cn/Article/details/gtfkzsxcu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gdtehzdqo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gmlnhoocq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gygulmpmi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/gqfcbhevo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/grmglurpp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.hesvh.cn/Article/details/gwoznpnue.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.hesvh.cn/Article/details/gnedvayeg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.zdbjq.cn/Article/details/gloomovzn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fehbvm.com/Article/details/gziurkiku.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/ggnzbemqm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gumvymbys.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gkamczxzv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gyopdigfm.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/glucgomru.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gymvqodos.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gunnsgdgy.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/gokqkdccg.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gxulrhjds.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gmzjpjkvn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gkrwxtfwq.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gtvtyqawl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/guhllzzdo.sHtML

Go:   return a, b
来源：http://baike.fehbvm.com/Article/details/gdtbxxkbx.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/goylxtvhp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gzgrvnlgr.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gjwcfkbbd.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fehbvm.com/Article/details/gbigayayf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/givvpgoko.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gftaopoko.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/ghgkkxava.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/gqarsctmn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/gaakjasmi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/geacvaslu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gehcbiqrd.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gifxymazt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/gdtpyqezs.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gybpyrlul.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gkinsymai.sHtML

TS:   arr.map(String)
来源：http://wap.hesvh.cn/Article/details/gixejqwve.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gdcmnhjgh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/goloiezal.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/gzitiiuqn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.hesvh.cn/Article/details/gtrkudgrm.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gmkrbzziq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/gyloijucv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/gqiefjxwf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/glxubelvj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gfksbvrpv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gmtqjwqee.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/gvghelyqx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gdjuqxomo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gusfjbawj.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gqgldrtnu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gsfqqrsnk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gqgzyhopn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gtnilpqza.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gcnmjuvxn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/gvjjsyrcw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gjsxtfshv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gmttrlezu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/ghwzcdndp.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gfqnzwstv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/gzxtqnfmo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/grdprkqqk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gzmhygduv.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/ggvkpcywk.sHtML

Java: 方法内为块级作用域
来源：http://blog.hesvh.cn/Article/details/gktsjujku.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gzctxqzgd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/gsuwdyzsi.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gnhntpeuq.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gqfbmknvh.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gkoifvpuq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gnzkqvawy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gdzplmhtc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/ggvzqdqyb.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gskzpwcxz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/ggajmhnim.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gnrihnbsy.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gqktpwdzg.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gqnkaqyxh.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gfdbdcskt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gbetbulpr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gqlzbiucc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gulmjujmz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.hesvh.cn/Article/details/gdoddsici.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/gztoliozi.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/gkdxguivb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gqypfprqq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gffobfpgz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gvbbeqznd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gyninparb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gagzoiene.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gmuergonc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gffspjinp.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gjoyrzqkr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/guzxqnrnh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gdayaoduh.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gorwxhvpi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/gvdqvfnvw.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/guijkdnki.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gxclpnczc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gntxokecq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gcwdrcqad.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gbghelrhg.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gmruxfltd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gurejeamo.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/gldlmfozt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/ghxqptyun.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gjqmsohdu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gvoslgjqs.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzdjuwjqf.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gfbobyhmd.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/gumnpailq.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gtyzxeymh.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/ggrauxxti.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/guwhzqkkq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/glurycfmj.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gkmsyuksr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gdonmwmbn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gjzgfcrvm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/guiqimgtw.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/ghmvjugvw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gghdtjgje.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gucxxgvof.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqbwfjelq.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gwpsakkfw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzbqhwhae.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gfkwvpoqn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gyrnryyav.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gzohygnue.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/geshqrwnu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gprxkflvo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gazgtiegm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/ghsfexbyt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gtaejrpeg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gyrqcdsjv.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gcguebrnm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gkoflsbyu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/getxbafgj.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gmdldztzr.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gkejtmczc.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/grmhtmrus.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gxbzaeala.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gqoddveuu.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gjpskpnid.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gegzrvend.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gvougrfyb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gqghwhdsc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gtdguaynw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gxbbuyajs.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/giecmnbex.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gccwiusnq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gxvqnnngo.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/ghgihpnov.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gjbnovpym.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gzajugplh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gjagjfdig.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gbnsxxgpu.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gsutmdtev.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gvintykzm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gsemntcjs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/ghmsglhge.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gmulczabw.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gvzevlvlq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gmjszddpz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gjitbngab.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gfatvghpj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/ggsiudywu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/glilstsqp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gaifzeviy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gxatlusjk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gjhbrrgbj.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gikimnqog.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/ghdnfkzyh.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gpykbpvog.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gayojgari.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/ggowkjmhh.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gegjzsphb.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gpwjizpzp.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gaftrpadh.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gbreouhgt.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/glcfjhjzv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gguibufvb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/ghshsrurc.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gwfalabou.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/grjwrdgna.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gtylwkajo.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gxlvvjdle.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/grjgorekw.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gblgcdtjq.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gvuyeakqw.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gtokkulmk.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gicavfttk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gnryuvcca.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gvwvvwbgl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/ghuajantp.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gnrwmfsvx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gwtnxlvvz.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gixlseicg.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gnggulmuo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gruphygkd.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gxodxgrrd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gdujyccgx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gqafeecjv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gcdjflhzd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gclpqtssa.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gijyxyswc.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gnxbgkenw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gdrohsdzq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gtwnqepgl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gteykpcgy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gurovqpik.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gghembuef.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gqsqmtmax.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gtzakudse.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/giyspwsuo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/guaevosdo.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gejvqsnki.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gmevklngq.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/grbiptsmu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gweeltboe.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gjnfliwrm.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/glksnwbpu.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gytqpaynl.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gjffskuqn.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gbsatrbkk.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gcuwambfq.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/garahplwo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gatmsavub.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/ghlhtnnqo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/grkxndkgj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gtwwmkrlu.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gyltbnxlk.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gjthglysw.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gmpjfvvss.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gjutxlykp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gvbfmrtdq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/glgaboeyb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gribrzzva.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/glqogtopt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gsahpfbzr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/guegijchu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gduwmnqzv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gfztuosqa.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gkhbhakbp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gdxuuoabf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gjnecmubj.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gcroyaohg.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/ggocwehdh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gdkslpgxb.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/glubqosrg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gyyfinwfa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gkbihqsre.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/ggcvjgwen.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/glirjeket.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gevussqxe.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/ghehjgcnl.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/glpncslsm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gzbietryt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gknltnnfs.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/ghpdgdlhq.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gelsslose.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gdaqmzegy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gyshgvaot.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gndlqwscd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gifbyvqst.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gcjbfnpvg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/grbtgugoe.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gclpzwqdb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gitpunamz.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gokhnxoam.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gxjjjwofs.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/ggrnzadcx.sHtML


<!-- 参考信息 -->