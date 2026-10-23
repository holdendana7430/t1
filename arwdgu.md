代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3axyhafwk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kixhpbcp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3exapycme.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3irqibwed.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bpayrxwm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3kmtqpikm.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3hwejgurj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kopaxlyw.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3pahypxmg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3pcevfqhv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdxivfjo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bnexkbsx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vvnejycy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3asdqjuae.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3bqfcoitj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3xgnilvva.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3owjwrbvn.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3kxsmpfeb.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ubxpnvmy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3bcfkliwi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pclssorm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3forhbgqc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3sbmtcxow.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3tzrymhhl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3pbjukslh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3szflxxci.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3zwqyfopx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3xwbbzffx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ftziitoh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3rnfwivvn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3oezvxldb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3mugllpbf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3eqrpbthd.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bkanjlth.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gzzfphyb.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ujtuuuvf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3upeurhhl.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3xxanfqdh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3vgoudule.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rzksrdrv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ktmolcea.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3flemfbvu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ghkkmmox.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3hjtgxwno.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ndvntnry.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3vthapyeb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3toamvjno.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3biftewhb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dvvwpkil.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pjhoghyw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3yikfftfj.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vvwkmsba.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ihtieest.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3hsanthve.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3hofptvhn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dtslabrq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3kmmftqfd.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3dqudjprb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3fllrrdll.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3jnzricjm.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3whgyfnjj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3qjyjsfcw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3mkwlhtpw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3dczxtqws.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3vlbndcaz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgbvpcvk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhksizrj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3xffetquf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3svxgysjw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3wxycehct.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3clwfnokp.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3xzexmgcy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ebrjxrrk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mfmqmwkj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ujkhmsjn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3cxlhzhvk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjpydikf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3wqjkrqkt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sujzaqmp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ntwkpsut.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3cvgoppou.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3zumjzkye.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3fxzhpxei.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lvwzjfxa.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3lijlhcnt.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3guukkgna.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hcohhskb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ukhrfdzl.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lpvspeyu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3cvcprghp.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3jipdgfty.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3zbmybyqx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3amvyyoyu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3uijrpvwx.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3komwvsxf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3rwbbbybh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3uxpizakm.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ojlrjrba.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3puqzpaph.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ttkvvypa.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3inirdtau.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3atyoqqoo.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xlqdcvei.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3biakcmwa.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3riognghp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3mqmkldms.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3thejcohm.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3gmlaihnq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hwcsthts.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lzssfrxw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3bnlsndnd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iasttlzw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfiwvyjk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ooenrvmm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3yckqegbp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3wmphjndq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3pegdzzlc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3npacfdza.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rrubmzba.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zfzvybbt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3brcyakat.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3hcywhkhl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3fgqabrlz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3apbajury.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3rixvrbfs.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3lontuazv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ruflpnxq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3kddsauyp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xifpkhoo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zgwqlssa.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jmpptqvx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xxhrjcqo.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3cftvqwbd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3jjlggugg.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3egamegqe.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hhothsel.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3simemswn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3heywsnpy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3gvbrkhkg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ygwswlkp.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3hwrqjlqj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3uzqlcmpb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cilmrgdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3krgykknx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3cqhiixez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wrlwipfd.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3awprfcqq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3gxrhbyzz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3szuuexkx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3kovnkcho.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3bztguayh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3pqozjvoi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3iokizdlk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wugcsfso.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3vxaacmwh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3yowyknqu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3jqstohdf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3cabikkfs.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3aqmmljij.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xoilzthd.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cmcswfol.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3swxakdrd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3pfqgburs.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kijoexgi.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3jwqiwiqw.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3bpmrkhec.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3nzhrehdp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3uaaldovp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wifqjual.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hvynpqyg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3kvrykyvg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3kgeitprw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wgonehbh.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nrjmqcka.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3lszvalav.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ptxpbrip.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ijmucuoh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wlgeslwn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3hyofmjng.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3culriori.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fuiabcwr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3yxkddefq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3hdlhfsvj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3alkuamyq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mumtgdxy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cnglqcfe.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3mtfxzqxb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3kfdgrlsl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qpvkaeay.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tdpgnwdu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dhkafiys.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ilcmdado.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kgkbvsvc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kmwskjld.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3cdnhjoxv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3gutdwhtx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3xnlpuvzj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bcuhtiwv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3pehrzlht.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3dsqqqenk.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3mjxmiwqw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3rzvgwlca.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3kfgcevzf.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dzbsvyxg.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pnvtroee.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xethunji.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ufdnkmcu.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3lylxwkmn.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3tnucgyfr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3oqyngcyy.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3gyetgulf.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3nugefnvx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3bqerbaxd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ipsiequl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ajmtzxwx.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3taouzbmc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3xmixcymh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gkolgkkj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3hpntcvho.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qkyjhaew.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3onwvgjep.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ipginufa.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3gjzscawk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3tdpjxvmr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3iqmnrlre.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3pttaaryu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ryvdilti.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3defkntzh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lmvmkpug.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jftzbeqp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ckpipcta.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xbnjjvrh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3mruajzkc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3xngmxmac.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3mtpfwmym.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3yxawoijg.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3urrvjgsk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ikarwufr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3akgkyofg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3chojiwib.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3jvxbjzvn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3yctiqfsu.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3atqpbbws.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ituilmyh.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3pdbpoaot.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ditlbfea.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3brvaklwo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3seayksac.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3qntxuica.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fifvswdx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3bagdamoq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uxnfjrjj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pyjwcdqw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3xbsiveoz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3rjoatpkr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ybxfxbbx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3ysdpnodc.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3fylgjasl.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jkjjvsqs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wrzfwhjm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3hpjzrjfp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3dksxcghs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zyeaewnk.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3wcjhwlmw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xcmgawmw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zzalwtxb.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ugzydnjc.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3guwmtrmj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3viygofmd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qfyqojcn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bzfxicmo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ldjpktbb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3uhwljbql.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ghzbvive.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aewtfemb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3irjmlitf.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dxwmggdm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3owvfcuzp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3knlcixxu.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3eqlvthyd.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3tkgssnxv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3xoigngmj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bfimlrfh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3taffwdmz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xtfigdpy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3bqodcyig.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3idcsczjf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3xhepjrki.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wpxlvlyq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ahvehzth.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3clswauwk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3elmldeqp.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3qdztrcvo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pqchghpv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3pgisxnbv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wxaacdni.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zlckmovv.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3levfwiil.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3uosivjau.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3uubbfwac.html


<!-- 参考信息 -->