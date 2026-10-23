代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3txjhoyto.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3vryrdbce.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3klhsrfza.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3djzljfqu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3japdgrxy.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3qkwrqxfu.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ugmnvkhq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3dvlflogl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3rajhqcem.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjcmlesy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lthwctvj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ictbcomj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3fybgutcm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3jnspisxt.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3kvoqvaqe.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3lmiwjatk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3hyfgifhj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3yadycppd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3uskvezuo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3dyqebsgi.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3bhlzitap.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3bnjibnvd.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xisafmpc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ykpkxdmg.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pgclxadu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3qcijnowt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3evciftvj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3kzvisjfz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3zulglmqy.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3rkqeqfgv.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3luxzvcqq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3gvlklkjv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3eqcnntec.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3bjivgdys.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3aucdsfoz.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cppspygk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fwhucokx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ejscqezo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wsyghyjf.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3aqoobjxi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ulxyydod.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3jeuwrytt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3browwfhj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xxsdapgz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3cmihvdtz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3uqwssfyu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3layrtbxa.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3pvopjvhz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3qvnmjqii.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3skztwylf.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3fyldyvvr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3tlpnjbva.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3poawfahi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jfewzzwf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqzqrzkh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3qkzmvobn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3bzzsnuzf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3pqjnrifk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mvwhrqrz.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3onmqmyoe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vftbkkvg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gicvytvx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3gqlphoke.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3peqzakox.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3fboasovp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3wdwjhedw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gnmzdbmk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3uwllxkga.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3tnxssren.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3bwahdvlt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3pgkfevar.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3bnqhlowx.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3zkwpywgm.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3woanuzee.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vcucelpt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3oarfkdzd.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zunehqfm.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3rfwphvyb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ivlgoyqi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3afrtimnk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3gojgomqw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3wxaxnxkb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3wmhhoyvp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3rzphxqcg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ncfhmnin.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ghfqbkbz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3iudzhogk.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3bnvuypfy.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3xfwcgjla.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3sjoqvxls.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3lvimlfal.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ipkrrtyz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3heotrfme.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3akvssmka.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3wbvvjxen.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3pgnemttr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qocfobry.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jqqxnbyv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3cgswkbdv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fatlmbtx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wajeecou.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3cgeytidi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ppijygil.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3aljzbxyc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3lxlypdrp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ueasecvn.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kjbnuoqo.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3iptaisnl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3akcctexv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fbdmasuu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3uczhjjgd.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3seduipiq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3oapjwwbs.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3rdshjkta.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3lukdpqis.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3butjvtjk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwnikjkz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3irwarcly.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ygwgpghz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dyervyuq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3acsqlejd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3olkdejmr.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3upqoxjpk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3zammxaes.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ddqkqncd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ruhfxbuc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3xvtjpylf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zpbwcbgd.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3mxjytkhh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3hupzmhkq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xvhqjvrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sadzmyvr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3vmvfmilx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hgrkthni.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wksqjlrb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3srhrwgbi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3fsvqmhvm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3suvtaqbt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3mcmyxluy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3lfsexppx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3mwankjls.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3hwvozpei.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3wnokyfbd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3wiqrxjpi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3lsrjqaja.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3pjmzfgju.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3abdsmvdf.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3epvilvmt.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ceoibfup.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3qhgoygee.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ujmmyfwn.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3cxwylwhj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3wktwryti.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3sibzjolt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3bqoenaga.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3klopdnbm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fokvpkwb.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3eaydmtdf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3pwvlbuvd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3mpcotbzl.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3sjrkhdsj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3uvqxsijq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3orsffirn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3rmpsakgv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3kehurvew.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3msxepysx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gjdozsof.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3tmmtvyho.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rizrpkjn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3avitcbky.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3lakcfpqv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3oxcmxudi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ptsezqcd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3anxgvimh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3horpepfn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3izebsqpw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ezcnndcr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lovjhfav.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3sjsscxuw.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ekzxzjwd.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fynrynqd.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qlzfrsna.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3fruknghi.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jwoguesb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3cxttkgsx.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pqrvjgwb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3epkqzcwu.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3axmxorjq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ptqhbhzw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ldmmgfiv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3snrcmxzk.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hdamfafc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ssusutbb.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rcnyrjlh.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ntppovzx.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3tqjjqcyb.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3fwurfcxa.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3xihvmxka.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3beyzntad.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3dyebwqsg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ztqkqtyi.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3jootzxnc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zeesbkmv.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3yojvumze.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mcuejdwz.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mavnnagx.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3jonxqgzz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bfykqjyb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3fpdejzwo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3xpgyexbf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3syppfzaa.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3kmxenvin.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wypyrqtp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wjeioovf.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3pszzzprj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3orsaoump.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pkvoeacl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ukdenubx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3byogofho.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nzimspcg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3vajxanjl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3sfszmyvs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3igfxyhvn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3jefyliel.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3nokremwy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3okzdqgyt.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hyixwiqb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3gdlesykl.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3bnutfaef.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3dzyenuom.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xqbhahuz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dypxkpyq.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ijzjxhap.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3uwupalme.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3amdahqdm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3hprskyyy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3offfmyfb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mmjsteac.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3cmpejoit.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eupdlvcp.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3vlazxhtk.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3qjxmhybj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3vgwxolqp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3aimcbajx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3yjxxnusc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3arppnlmp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xxujdxwb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3lupksdva.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3shmjuxmr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3bvbuajyn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3grgeguzd.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3allrvavn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bnwrtpmz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3algafyvg.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3zqoprvqh.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zqsbbyzw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3khbsxpyy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mgnfsgad.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3awrtvxih.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nhulmnnm.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3jgpeglgc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3kwwmsjvf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3calvxhas.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3swckhfvz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jdrnncis.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3uahfsger.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3uaicgxur.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3glueyjiy.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3pmlcbaxn.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3aabedxip.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aohjfzqe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cnjygyol.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xcgvupyk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rfmrwbgs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3jtvabayi.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3kdiknman.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3aprhokqn.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3imxekmgx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3btzmkdjt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nekccdvm.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3grvozlpb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3lfawxsxc.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3acombmdx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3czpdjadc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rigqqqev.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3qrjxpzzl.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3btbfskmj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3upmvhgtp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3mazlrrye.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3gtsahcsm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3sirxqbac.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3jesfyasj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3gzyiiujr.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3lsmhpojb.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ltwjcmgn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pyjsvfxu.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3hqphpdpz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fjchydlo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3bjnwfwbd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3qvbmmgtf.html


<!-- 参考信息 -->