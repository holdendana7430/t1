代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hawmwqqg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fvrgbhpw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3enghsyws.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kaposplc.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ankbaibb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3uoctjcrx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3klfyxqep.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtcozhhv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtakeidg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3pcefzugb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ylmcaerg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3rvpgxdgj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ccmmcgvc.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3vbvumnuh.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3hdsljici.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3iabgnnse.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tkkqshot.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ixlyqhya.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3mluuokqf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3cveqbjdg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3xjxlggvk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3lzxkpowa.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3slsalpwh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3rzmxchlp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3xneynkhk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymcueomf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3yktwfafd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3exiwukwp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3wcbifwqn.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eegpexzi.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vaiowrai.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3owatllrj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mskhbphu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3plyznnek.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3jyqoylsk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ttigxpxj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3epoirotm.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3uhfgdrwh.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3yeegvqkt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3mstiqurs.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3rowwqckv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3dwdhvjhf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3hrkbwklo.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nqfpnypz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3aswcgytr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3sinwbnaj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3qpndrppf.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3mgjxoifu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zrkezoxi.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3cxbybrtr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3aupuixsa.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tpmjzlnb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3zxqgetux.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3luaoaoto.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3hnrvvzph.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3mleaanhf.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3srbwnphv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3wpuefhjr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3cubcghlb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3immwrvcq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmkkclmp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfmoogyu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3tqjigvwy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3evrifzvu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3twzibnqf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3frxfzbio.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hrldnwst.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3emobzunz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pwewbeag.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3hbzkegpc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3srkscrtu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3qtovpvzr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3pdwrtjzv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3hhxjlmwi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3joemwwqd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lojkmkkz.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xwcxxybn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3clwvaznn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3sdyqgglu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3quzykddu.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3dldnevjw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ayovqafj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3liozplyp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3wlqpawac.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vudwgszv.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3lmfzblno.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3tcyvcpcc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3cqttxivy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3jqaakbrp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3hygvhfwe.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3edqmljzs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3bbtqnixz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3xusukpup.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3xlvwfhzj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3wpipglpq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3akeqogjz.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3dndwhlij.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bbmybixt.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fuhpiahk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3kjqclnjw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3gtzhpwmp.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3rbkijrjo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3uuqsgowd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3lnpxfsch.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3uswbicsy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xviosmvq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3qglheoqw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qjoztoup.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxpcxwnj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3rkvhfjkk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3wtdiqmsj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3lyrwocxb.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3yilqklhw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3lwdkgnmq.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zfpkgvud.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jvomvixz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruolkbsw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3rhnmvysy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3edjwfluv.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3kyoxpfth.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3flakncuw.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ucmbmupd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ddihrrra.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3zzjoazkj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3sfurbfsz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qgwggywd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3porodicf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3msuetejg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3qorauyzg.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3igsfspvy.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3bnmtwfyf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3phlqjxcr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3yzlvpwjp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3leskgciw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3fegbrgib.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lhpcczou.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ornnqbqh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ylpsnhoe.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3woyxpuil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ywwufvev.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3urbezbol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3epwvekhp.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3euhhxnxq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3solnqtxs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3pqrsiwhe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3nbvweywk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3flsgnuyf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3liymgrse.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3aiavadxu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3lkynvhxv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3jjeusfww.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3yybhluvu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3iieanpfc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vkkevvsw.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vklbltot.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3uscyrtko.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3xrczvpou.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3efqhbxxd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3iceosbtl.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ptgaxjgi.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3bcjidncr.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cydlwowg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3cdidcbkp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3mtfvhhuk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dasnvkta.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3aybdoxvt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3aqvingfm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3rjfxykuj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3upmisxdc.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zepurbtl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3yscwcrmd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3shabaxoa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3fjkmckux.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3drbommvl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3aliwlzdc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3mprwffts.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3azqbwxxk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3uxrogyrq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3miyxdvwv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wyxpcgxc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wmijcgjw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dcpoyrtq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3qlalrrcw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3wzyjhlqr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3smlojscu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mzfunfgu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bobrsuad.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3cupwozwe.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eswgnlfs.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3swbehtia.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3bjbwisnl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3rfadkxiu.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3hfbgmvxt.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3puvrsxgt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wluamnbg.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3mesokmbs.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3xtgcrvhq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3uairvizw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3tiryxkmb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3sdxdfmjd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mcbqydqv.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xqjlwhtq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3hfsgvqvx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3cidkfzat.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jfdghknl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ipqlkdzn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3nyvxefxi.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3kmorvzie.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3nyirnwgn.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3hjvrncjb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nxsvckem.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3nnvkkiwc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3trfwsrre.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vkcfxdcc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3sunpqikt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ygfgtnif.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tgjfyjuz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ntvfitur.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3gngmkild.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3lmatpgko.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3javvnlnn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fwhixdmm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ykoaikuq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3gpxspzba.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3akfdktnk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3tswizxtt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3posqlarc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zfejsdqo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3izlzeadv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3nvglwkad.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3gmyxnyvx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3xjrbayhw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3goiojyht.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3vgqtzazo.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3hykadnux.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3wjakoxnc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3cucsxqbh.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fujglscx.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xwsbtrwp.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3zrtvvtor.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3gmjrpdan.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3iiayrppz.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3abrjipfn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3thirznau.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3alqjbolf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3uuurdnpf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3kffsxwjp.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iwmllihi.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3uqqonwft.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3hdilkisj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3cmxhjztb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3rsnndxor.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3iwchayrj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tanqtabf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3tvssjypa.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3elnlhuax.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ajpvuwuj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3cldfglgu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cuzeqcqd.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ccbspcun.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kqslqecs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xiqvokjn.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3bkgjfwen.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3fafwjoqh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fektyisv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3zzbsmoxs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lmpfayma.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ctdpijsh.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ihodesbd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vvvlqrwi.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gvceqwla.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yqwuomsr.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gmtekwvn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3sxptpghf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3gvxflxlp.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3veadxwek.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tghxdgez.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3pmltcvcz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ipjnmkis.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nqrptkxs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hwgqktql.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3zmgyywwd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3vtwjxjib.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3wggnnnrv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3lzxmylcs.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3kdsobvgi.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3qjylynxq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cjpeorzy.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3tazxjjor.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3dmnwwhkj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3euwlvnro.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3abaosfmq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3huvbagpz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3rcimhcoi.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ehboybvn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3bviafufx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3mlkzeaiw.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3tfanbiqn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ekjmpguj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3vlsshapd.html


<!-- 参考信息 -->