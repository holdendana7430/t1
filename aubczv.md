代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3goroqgvz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3stnsjmwm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yijhizes.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cgyanrbg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbbwzhmc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3hdnykaea.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3nrkoaruv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3htetywki.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3prewdkaz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3esfhegdg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3jlkoxpwu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhpdzlap.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3czmitdnh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3unqrrtqe.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3kzzkzzds.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3dfqwsymb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3tizlzlky.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3rlqmifme.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3suxikckd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3mvoigsvg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ijshakgl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3chhhsoht.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgtfhnfv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3mpjchhqg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3qwscddjv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3arrhiozu.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3nmzwptcn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3hpdvatmr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3peyxptio.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3objstuvk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vaqaxhtg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3tlncuqdq.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ciozxhrh.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3irssjdsj.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3adnssvil.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3qaywmexv.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3satzbzpj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3bqyjeueq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3unbhpkuk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3kqakdmhi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3hfnikgju.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xgqmmavf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3oakzrzko.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3fymfigjv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3sqctzhzt.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3rcmxhjyx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3mouwxvzx.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fkamlzks.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3umeeppxz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3pcvhvhun.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3pykbpltc.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ymywcseo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gwyfctdb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3wdliqjkp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ktngfkrl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bvnsqorh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ocdhpxhi.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3hkeynzcn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zyizdajb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3vqoxveap.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3pkiqclph.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3boklruwu.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ccuxjbgp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3kjaebvjq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3yojnughz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbkzikyp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3uauhdjhc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3komuvxks.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3sqvfiuln.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3zunioiop.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmjmpjki.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3fymdzysi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3nhlsdcbt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gkpwifpl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3apcwfzbd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3nmggzdjl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ctglmgdf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3edztjoeh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3oizbegwz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dajlavwx.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3iyxltpcq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3aemhathv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3zpbylbsx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3irvngwjo.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3evyigeme.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3pahtubrm.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ukexcixj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3fcnsoyfv.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zdpwbeya.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3dnsmwyti.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3wwuihxux.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3mwuyjlnt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3abhqrkze.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3skuoyvco.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3tzheeade.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3wsivcqob.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3opahxnen.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3lvlfiipr.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3tojcvpmw.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3hpdjpcdi.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3zeiavxqq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hjixoedo.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3spqhpxbf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3jkgfqlsz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3trsxoasg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3kovlymoi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3drerxvye.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3slactcbd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qqavxuym.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gubytjjw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3exxzbecp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjjzpnwt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ydwsyjfo.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3irzckitx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3hleftapp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3uwrnxyew.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3mtzmpbvu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3jeeplsvf.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cwhknoru.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ggaskbnb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxqruisu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3isixuelz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3bimtvrsy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cyhynnff.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3tvzedyfh.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3hdomiexo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3powmaszv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3knaipehd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xxrfxqbh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tuujzmzz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dnnhhcnp.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wvqdgnhs.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3smvffsya.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3laeidjzp.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3mvntqhhl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3iwlrjody.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3cjgyygxk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ayosnmms.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3iohinrqu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wtouvcha.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3nfjzyepz.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3lzmouhyk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3mlwubyzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kskcxmhg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3oxtplrrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fylrrjmd.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cbpkjkli.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3oogtvijg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mkonosch.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wrflgrve.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3uvvcitwg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3tynodyzn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3qoccwbfi.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vpcdbxwk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3gkkmdspk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3hqafbnmu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ecimblpy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3etzwojfz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vipngcyb.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3oczayqvg.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rrfoogtj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3owdaknzk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3dlbpqpnf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3tdapybvz.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3mbvzxjzq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bwyxuyxs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3wfaaipjy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3kpdmeyzg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mbldwhay.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xcxprfra.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3zlzywicz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3euzdsqrg.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3szqolkvy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3rfyjgxnv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gqrlkzqh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3vuzxlbxw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3yvogpiya.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lqvobhbc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3jhluzhpw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3pydkpbxs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lhaakljt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3jxjtwncf.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3juhvagth.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3atxlluri.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mhvmugvv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wycxqaka.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3fkqvdeat.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3wxrjeega.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wxyxwzae.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gldkcewa.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wvnmreyt.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xjzvhbla.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vcrjlnzj.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yqgielsl.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ldpdjnag.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mzwnwrfs.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3itvmlvng.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cpzbxhfo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xwpysxac.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3prxeilzu.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3sbdbdyqb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3mzrirreb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3iqzbpupr.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3peruombo.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3afwqmhcu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rafrcvqq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ivuyuzbn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3cowmiplm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ivzdsuor.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3wvjmhggs.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3qqgbdadw.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3utsgklyq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3kgllqkao.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3bjasdeyq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3brkxuvhq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3bsqdwzbx.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rucjblua.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iqtvbfoy.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3qrbuiblh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xwcbhmkq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3eujynfab.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3hgkekcmk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3waqopvho.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3crqobnyf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cutdheht.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3wjerkqsd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3xbjjgymc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ucsdldbm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3smqbtjaj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fobynoeu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3yhbeuauf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3snvuznrh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3podaoaco.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3mgmxtpqn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3nyvipycf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3pvmpycff.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3bpfrnncf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3mxpqebab.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sxrizeeg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3bittmlgt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ftssphdu.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3eoqgvckq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ranvnrcc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3auggfkht.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3tqcsltsa.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3jyeyhdgw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3drjdlbau.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bsgknbqc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rnppnscx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gbadbyci.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3yrckjotn.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3srmuabgv.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rtjemfyn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3rpozznae.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ubsnrbnm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3feiqhiqk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3edxfiiid.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3eczfyimk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mqkxfpts.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3szzjgeqe.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3kafcqzcd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3tikprpzb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3efxskedo.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3qntykoml.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jwmmdgfa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3misgybhb.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3zkwofjzv.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3znezdexm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jpyqyvok.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3orhpoxyj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mfarxevf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3woghetqd.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3vkxnxufp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uiclkrni.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ekyrazkh.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kfhkcdcw.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3avxrdkdk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3cqehztve.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3qukbcdyr.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3akypntjh.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hcbvtfwu.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3eqnsddqy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dkemfkzm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zjoqjfcy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3caxdkuyu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3trkrzdpo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3qegdxxoz.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3hqjhipyh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ynwugwom.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3wlvnvned.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3qwrtvtxu.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rwriygty.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3xkqgxrfj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ekrfgzsm.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3jvlmsdhm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3zlhmqdgq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nikhcrly.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3imjienfe.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3wgmuktwh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3xlznulmm.html


<!-- 参考信息 -->