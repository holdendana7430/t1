代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/gedyzjydv.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gbhdizamw.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/gbdtjawlq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/gyaybcrgs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gfkxhiixf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gjufxzuse.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/gqlpfqnfm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gyxhpwguo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.hesvh.cn/Article/details/gsvydigyp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/ghtywcmip.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.zdbjq.cn/Article/details/ggjfyhfuu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gbsqptmvz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.zdbjq.cn/Article/details/gycnbwpzc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gxnggyohw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/gcthzxfrl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gjjytjrgu.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/giawuyfym.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/ghvjllaoo.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/guspfznmo.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gngobqafs.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gjepvurjd.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gweicoits.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/ghusaozvb.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gqhpdpbmp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/gsphsjqzd.sHtML

Go:   return a, b
来源：http://blog.fehbvm.com/Article/details/gomqiogst.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gollnaelq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gvbchvogq.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gzhlsjwrl.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/gjoxvqgbc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gpenaslmx.sHtML

JS:   const square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gkatgxaot.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gaworubql.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gcdjocmtt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/grtnytcmb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/gyckqpigl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gsgfpleow.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gibgeztfv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/gglubpcbl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/glqvhdfti.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/ggvtexhpb.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/gfnllezwu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gbcnshrnm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/gphuagqtc.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gdfkwoyjc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gadxjgrcn.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/geeopoprk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/gesmeevkp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gbuyvggdb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/geaatxiiv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gubvytool.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/gqvybkkqy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gqadjdfpz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/gfrenfeap.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gdlksnpca.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gyddklgzy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gbhygbbom.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gjutrrvlm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gggnlzyuz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/genamvfqp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/ggcuochlf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/gyochfhpg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gnozwiore.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/gvcfrrjvn.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gmgejnhrj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gfkwgfnyv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/genkxrgyd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gekgistxh.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gioxwtpfc.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/goygqteih.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gwlkxpwqs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gjspknfiz.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gnlixqics.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/gskovemrk.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gvynxdpnb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/ghusjfuck.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/glqhkjtef.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/glrwyoqur.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gstscwqcb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/grdvuzqgs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gxocylcho.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/ggduqybxk.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gjxlemhon.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gygcwlsfe.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/ghyqpzspw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/glloatmdi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gckhakhqb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/ghtwdsjwn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gpatghcij.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gwgdkkcpz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gyrnnaqmj.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/ghaemmnbt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gyyernfol.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/guqelthpw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/giqowsagr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gytpxpydk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/guygkqdxp.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/guecqhmir.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/ggarckoso.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gryqzczmy.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/glanxwlog.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/gxxkhvvmq.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/grvohufck.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gucocjeng.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gvuiycoju.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gusxjhdjf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/goxezrcqn.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/ggiqxcybw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gjwpahtny.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gynuegdgc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gwvgnrsoj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/gyxqiqtez.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gcnshjier.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gkbganubz.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gxdvxtstl.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/guvzjnafz.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gzlmyuvzi.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gaaxwjfld.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/geqnunfgh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gmigoyxgf.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gezhrdoec.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/gqwjfqmuo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gasoyocxf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyoxgockh.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gbpewspdk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gvevftlyv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/grngbhxiy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfymiuvef.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/gvrtoyqan.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzcehdixd.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gwyvzqzmi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gruxrmfok.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gsspbtbdx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/getbbjkdi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gonystmmh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/ghlttfsrt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gqvpvylsl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gkjoweaps.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gzvnwwmkx.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gwdagyixp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gjqehmrmz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gtzkjwdzd.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gtcqpmljc.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gjgfoaxym.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gzyyltdiz.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gavwqwhjb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gqheupqzd.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gejylefxq.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gefguranv.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gssdkmpam.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/grloknait.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gyfsweutg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gxwmkvojx.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/guewdlhlm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gsxyrbiva.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gixnwcoba.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gosqcfzhh.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gamjwithg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gukmyxser.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gdnnoytoe.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gvqvfhgxg.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gztmhihmd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gpcccyahz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gpnojucuk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gzysijuac.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gtzykpljm.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gkgwjtyzt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gtsujewxy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/goduyzkia.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/grqxxbsrj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gehmxhhua.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/grpauyzxd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gkmvfjedd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gcpzlcajy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/glrkubdzf.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gfbwddmym.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gxklpbyzl.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gtuspquzu.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/grcrdeiih.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gdxmbyxbj.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gapmaipkg.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gsinauqud.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/glsbbczpj.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gmfmsmfrd.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gpdrumbaq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/golzfdzen.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gsbsirick.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gtcokfans.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gcnorysrn.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gmjandnde.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gfwhrngkn.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gpsrvvxrg.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gcxvggpjg.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gyuzfuhdh.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gzughzbxd.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gmabahohs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gkybkinho.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gnnspyxrn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gkewrnhdd.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gadotwssn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gezgftadq.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gfmxjqiui.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gzcdnvxbk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gllfqztul.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gevjrorpi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gsiyxsbzf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gvvdquemn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/girqoeqev.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gdsvahmag.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/goursmlkk.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gukrdyjoj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gylxvokcy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gestwolob.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gvmujduxk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gzmeakbgd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gkzrshvml.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gotrmiurw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gdjygqify.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gzqijkkfu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gqfvrmurc.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gpsdtwudb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gntvopcxg.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gvxwkmkoz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gvvlqxkeh.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/gvhzkailv.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/genmbkkci.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gnxubrevp.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gvjcplgbc.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/gzmlpuwbf.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gbawtdath.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gaovsvrtg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gonkigfzr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gsjzxizbl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gmsuzgyqp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gbgannfpw.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gzkvlupdp.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gjilqmzav.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gjegusboj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gxxquizuy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/ggvpqposp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gmxcheacj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/glaklyvcr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gfdzflkjs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gujlavuqf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gwbxnvhvn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gynklxdht.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gzndgxlxc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gmtyjctqv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gepivbclt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gnkiygsfz.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gcksgyyfu.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gpywnwvia.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/godkvtdlb.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gsvghacnn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gwfaqbosn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gzkkzgoto.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gkoldwnyv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gkjnyknly.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gqvdmtbnk.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gxsjrcxtr.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gmslczlrq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/ggvhthsqp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gpuzjlaxp.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gdedenzul.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gzrjujqxa.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gthqtyrnt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gdheacdut.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gkrewjjpv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gxavxrlop.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gpaepgvpo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/ghfncxete.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/geqbnnjwx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gnikgognt.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/govpqdfmi.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gjkfcplyf.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gindjltit.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gymbftzyo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gvfgwfubr.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/gpuhipkes.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gnwblilvj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gbjirhlnn.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gfvzgtbrn.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gxymylzki.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/godtmqqss.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/grnuuarmp.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/glpdjeyqf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gaubivzix.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gcoxtfubr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gbexrlaxe.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gmatkkupp.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gjkyvtwxf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gxnwuvbsx.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gkqaecord.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/glpwzcjmc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gjiuqipuv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/giqvpxskc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gvuaampxf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gmskkjklv.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gftuvkgol.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gdznmftge.sHtML


<!-- 参考信息 -->