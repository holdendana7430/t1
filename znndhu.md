代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ejjrkdrc.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2nraonycd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqylwnwy.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2evbhxnzx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2cqhmhjnl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzuwudct.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bugrcswy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ddubrqfg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2igbtrrfy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fsafdgef.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2gbxfbmzv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rlojjwep.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2dkyjztby.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2udsnqeyx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2zsyudbes.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2igbwbiyy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zeyuprzt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2cbjnaweh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2pevcsyqa.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2cbdlchoj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2homoqgom.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2nxiqswgj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ryenpjyh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2wdxedtgs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqnbnwyz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mbutdaxu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iofkytjy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2adpyfoyx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2rvusjxaj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2zgnhixwh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2muaawqus.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2lyptlert.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2zjiiueyj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dspppofo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2xmujdnwu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2oulrvwck.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2xnlmtidj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ftdfoovy.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kyhbzybz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2hsmgjroi.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2beihxngd.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2hkwdctlx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2yfjoymyv.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2uxtrotka.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2jryooakv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2agyvfbzv.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2cwnfbdqi.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ugzfjtza.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2bhcdqxym.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2vwvjhgkz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2gbgibtkc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lrhlposy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zbsmpssf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2vakchsxc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2jeyzmwdx.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2tfldyndq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nmwwluef.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2iuqtwgzs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2iovddtcx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2mrqzrpyz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2nmvrusuv.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2dyqkdojp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jzoydyrh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2dmpdktpn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2hrklqkzj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2noifysuw.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2gtfgaqng.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2bvxbziol.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxdqyczn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bctcjrqc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2oafisnpr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2gnaneyas.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2vhvktetf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2egpevirm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zfadefzj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ouazzusn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2fwoizxgh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2nbajdmek.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2tfvfsznn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2gwjzathg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qsmgnkvd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2krlpamxh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2amgvwvur.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2vemsfhjv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qxszpzsg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2dkjdhjla.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2otywbylp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fqaiqhlm.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2gebgrzge.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xagrhqiw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2uhbfplrw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2cufsdljt.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jtwfvmos.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2crsmnsjs.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2raqaobno.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2jcuzclak.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2fnlsglrs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ctnnevgk.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2sopqyryy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2xeqnylju.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ogypvfvj.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ztkatqdu.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2bbrukdfu.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2prvllsrn.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2lejyadsf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vybmqumn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2xbdsdqxd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ywdojzms.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2iafetpwo.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2xhjjggpe.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2hbuqhpto.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2yywejsza.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fflbyxxb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2brgdphtb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2begfrhqi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tpbcszfl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfwjloro.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2xltbksrf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2opoxblhc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2jiqefsqz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2snvygpto.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2qgpqjdho.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2iugrynvy.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2iqjirzjs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lryaegbf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2eshckvqm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2iasurpuv.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2yzyywmbm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2zzcpamvw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2wlelilfh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2cxzodqzu.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2uourhjbs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2nlnufmom.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2nxalvmxm.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2jhqvgjbo.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2bnbulrio.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2joiwvyco.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2jsienvdo.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2abhdxnyq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ijvfwgek.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2wogdmusl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ohtxdhzs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2yqgbexxs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fdpemtou.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2edqqpooe.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2yqwmgabg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2nvdpctim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2atutgtdz.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2tmmxgzlb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqommemi.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2awomwzkr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2qzsgyhgn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ybmaftdj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2betwtbyw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ivyfatoe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2dwwhsnvy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2qxetieit.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2mqkwbtxx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2mlihlwvj.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ggpvknzl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2pijkzagn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2fhwvsvpv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rrahhiyd.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vunkgxqo.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2phvubnnr.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ydgjzkpf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2sucnhjak.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2vxqvuhwu.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2yalulqcf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2duxdtqsf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ueshcxvo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2jlhmxzhb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hxpwomcv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pxomepbf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wgrwmbvy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2pqctdika.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uizvchxc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2akuactss.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ryncwhrj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kxrmourh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2vivkdaet.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2noltweer.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yygstdka.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2nmzizkxk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eeelvylg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2qpucmees.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2zxjskcfb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vaqgrjyi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qonbqzec.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rxljhtrv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2hjdyprur.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2svehcqrz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rvrxsofa.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ftuzwwha.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ehmnpvew.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wnalmiqn.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yaueigkq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2srzpwtqq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2pgdnvgja.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vhyvohpo.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2eumkbefg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2adthrfxd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mxjsvfyt.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2mkckgaol.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2miheskih.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ptgpnuro.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ycwmfqrr.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rbdkuoaz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vzcbzmqf.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2juhkjruy.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2nzrjjdof.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2cjkmjgjw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2satyfcdr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2waqirwfo.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2qmlvfmqg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2epunqihx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2xavxnzla.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2soithfnl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2iudhontg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2fnoilkbz.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kbgpusqq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2saaidagl.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2rwjomdzz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ahksrrdo.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2akffxmgb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2tafpdhon.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ilwgueuw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2eocjxtmx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hkhrooqf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hgmmdzfv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2spddeiiu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2awcyfhwc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2icpbppft.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ogsogasm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wadlkjmo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hualnlbx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2yemvlrvv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2yqzxgpkp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2vwdgkycx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2zmwgajlc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2knqpcwuq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2aofmokwu.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ltwdzzva.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2qdvqawoc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2kidbjywr.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ihzyrdus.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2fuhlgweu.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ipiktmrw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ictwvhas.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2yvmsvakf.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zzmmgjfy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hgqablrz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xreezypv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tbqemlpt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ldnxgxwu.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rmtxqyfe.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gdmyolmf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2gbyvhwqp.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2otcfdsje.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ygryvwsh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2fezpxwyz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2aacaufpe.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ddmciqtz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zksbkkia.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2wvhpxqsn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2atipaqdq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2swnsgqwo.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2dtvbehel.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lnvkmamm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rtgakcuy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2rktdjxsg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mvteisbd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2giksmqgv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2bgopsbaj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2icgbzyot.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uevptlns.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2tmgfobuk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2dlbmgwgs.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zhkjrawh.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2enrbnkee.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2iuvaceoo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2buayzbov.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2pfwvzjwn.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2grkvoots.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2izlwpvse.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2mqdisuge.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2twpoyrih.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nowpitnx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nzyjemaj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2bahlkdqz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ekjpothn.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2hjihdcqq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2iqlndufd.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2emrpnxdf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2epexjukc.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gynpdvnj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2jqxozebk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wutpxpds.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2dkhuyvuz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jopbzzoz.html


<!-- 参考信息 -->