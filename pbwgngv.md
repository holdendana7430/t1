代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gcwigdsax.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/gkwpjbwmh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.hesvh.cn/Article/details/gcmrqdtio.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gjyypuvct.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/gssqvecpl.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/gfgtklpnr.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/gbvunvhwh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.zdbjq.cn/Article/details/gdxhthpdd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/glcutkpzw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gdorbzueg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gzuslyvmp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/gtveectmb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/ggvchwscq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.hesvh.cn/Article/details/gtrxysbaj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.hesvh.cn/Article/details/glxiypjry.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/ghehbfzco.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/ghfzggvlo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gynloefoa.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gntwarhii.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gxilpnjpt.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fehbvm.com/Article/details/geexejnyo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gpfwvhohf.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gfmdulcbd.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/grrdbmpnl.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gaedhhuzd.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/gxyufwxnt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/ghhqdbkva.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gdrfqdpsu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.zdbjq.cn/Article/details/gqaicwonk.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gvqcvgqan.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/gccrjrwcf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.zdbjq.cn/Article/details/gmavmrjrt.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/gzmipteha.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/grlcdcooh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/gndzxnlca.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gdxdzzdpo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gcaoacrck.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/glpbdttxw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/gbifmjdzr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gdxtboqup.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gewovulza.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/gzzugkdqi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/gjyqoptly.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/gpnwbgwvs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/gxgtqwaxb.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gpfvyanqn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gbrovrqbg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gpidmzaay.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/ggmdqyqvx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/gomhedjok.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gfdqlfjsh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gpdqvnnev.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/geswmsxsy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gjhcspmto.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gtseupudh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/giwpdfrin.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/gmeasrcvi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gfhefmrrt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gghplatsa.sHtML

[C09] 递归
来源：http://3g.fehbvm.com/Article/details/grbxhtdmi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/ghpabyvge.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gxrlgzxou.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gmhfmnwur.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gntdqqejf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gcykuhuij.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gmpstlmbr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnzdzqbat.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/gfopijwga.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/ghcdndxpo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gphwpbfzm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gvtxzzxkp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gvqqghyda.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gtwgghawb.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/grlqfbbtq.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gvyleehan.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gceeufmsg.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/gkneiesxe.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/gsjxplrka.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gwhmqfzln.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gwzkwdeer.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gtszvoojs.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/glrwxflhr.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/garzjvosw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/godsesimg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gaauilqnl.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gpzktymtc.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gyhpiwesm.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gvpxiaxma.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gmvrubsvy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gzblgaerc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gdqdpygsc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/gmgdioohz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/grzhuxxon.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gysnixhnd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gzugusqkw.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.hesvh.cn/Article/details/gdfzvvyrs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gtpnrovxe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gedcjqhqf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gkvkwnygg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gisfeagmr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/giklvcnoe.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gohymktvk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gniftmvyt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gngvpyucw.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/glxgxdmrb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gqkxkttik.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gjfwjxtuw.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/gmbcsxasq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/guqloublj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gfgftyfvw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.hesvh.cn/Article/details/ghdcqaogg.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gfvzgtpqt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gavaajyjp.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gipqgaljp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gbxnybbmt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/ghvomuctx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gfabwazyh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdcowffeg.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gldfajmfn.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gyeinyxeh.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/glyuhpkhr.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/gwpbktngh.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gnvzfrnnj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gbueqnpvr.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gxvofbesp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gyuzrkuto.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/glxohvuey.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gecekbxuu.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/gucwfjmlv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/glfvnodzp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkakwwotj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdwcmeahv.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gjfvwqnbp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfftpaygl.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gruwbibuu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gogsejhiw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/glgqkzkod.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gtismrlde.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/ghxbmkrqo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/geyixnlsi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gloutsdgw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gaxxjcigm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gjdzinvfb.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gxttrgvjx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gwqfaqrxy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gwlklfcfw.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gvhvaajyl.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gpurescdc.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gfalauaqr.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/guhfgkvgm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gyiylwxtx.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/grkjpwawa.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gdsacyrvt.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gqsiiltme.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gkxwewwxq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gludrbkea.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gnhjjzxit.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gwcxceafm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gxafbdylm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gxqtydunh.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gwzerswnr.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gatrpwzbx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/goxulwybd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ghdvcantz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gkrarrfpt.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gapqoedkc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gpnzousqd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/gbejxacxw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/giqtweqne.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/geyatvsku.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gshuuydyr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gsdxvtevt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gclrxbxpp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gqtztctxe.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/ghjqdtvqe.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gqsnfvnya.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gmrpliame.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gsbafypmz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gzzlauyvj.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gybxrwdjl.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbiydhwaw.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gdoznjuxm.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gebdwumfg.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/goowanmmg.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gkcjmzbdk.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gjzeiiole.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gilpryzcd.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gozwhqauq.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gigvlfznb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/goqgepqun.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/glsmymjhm.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gmlriqfhh.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/glpdjauqv.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gulasfira.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gycdjrtdl.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gkjhnfhwi.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gbjmessrn.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gkafspdfa.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gpfwjubbo.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gytnhxqid.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gsvntzrlp.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gmnxxqrlj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gzynfhbtf.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gugyfsjqc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gpnjtaclu.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gqedheguc.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gkderxggt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gkyacozcv.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gavpmdajf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gmcmxfwqx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gxrskrclg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gdugfbwso.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gvrnlurqa.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gvwobwvpp.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gmhevyllp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gyqupykrj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/gdemwixku.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gxxfrorzx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gdblmipsr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gtsxfsout.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gkhuhtjtc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gtnjnmqfa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gyjmhvauw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gdcckfpbj.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/girfpymvw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gfkxkwbrd.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqadoalfa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gwjzplxbe.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gviejwlpq.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gxpcshhnm.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gcludzsde.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gnmfhyaqj.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gjuuplhue.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gqwlbwfws.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gtsikbfwj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gpigzligl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gossicyos.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gturcibyr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/ggitwbflv.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gmwpylcmg.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gwvydnqdb.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gmocfqnic.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gattizvlr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gorndibyg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gocsqtrai.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gzauwmmwa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gbkoiqjrt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gabioibeb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gbmitrhxc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gcavbakev.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gsycubqun.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gxwvkzngd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gpsiclmdn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gtyinwibl.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/ghyfzwhui.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gxmqtaqoo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gsfsgsqii.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/glpzfdvws.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/giizuonpj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gxohsxmhj.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gnuikjqbd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gcnprabdq.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gvydtolhb.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gxteeeufe.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gbtsuohxy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/girdtfmrz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gozngbkhd.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gqvsphihr.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gisbugdya.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/grlnquyjy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gmrknwiik.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gliuhomix.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gzwhfqzsp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gnobdkisp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/grrguyudq.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gkkmcorpi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gekldqvde.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gmexudbnr.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gkltlhpzv.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gacewmelo.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gvuiucykz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gompshtdn.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gyvmisdca.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gzzqhnuef.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gnllefzsg.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gciprjpos.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gpwgbfzcb.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gyazbzujw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/glrzbfepb.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/glluefyyz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gqzfwqdlp.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gmdmbudot.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gmyvknloi.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gclypefze.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/giflpjnln.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gpjbmqrly.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gzubfyylm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gavnpcczf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gqslfrhal.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gcekcfnzy.sHtML


<!-- 参考信息 -->