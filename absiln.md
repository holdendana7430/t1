代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2gpzrtqfw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wvvukgts.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2rcaqolyi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2counntpw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2glkmnoey.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2xogyasqp.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2musjgltu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ltzrzsee.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2muidiacw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2lcrabukm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2epxpmuyl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2lnibgyvs.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ufntdczt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2robvgisx.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nmndjusx.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2jehcvejc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dsuybdip.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2eutxlqnl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fwfzteof.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2nxovoatz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2uvmdbefp.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lgcjxkxc.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tjdsrfli.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2gyxrrlwo.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2phrcudcy.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2lzeqspyv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2usyqzzix.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2msjjfmkb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dzcqdsxn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gvljuxzj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2advwxlyo.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2szlccjng.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wyfsgpbs.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2xaqtrtep.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2yjsenmiq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fapbvsea.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2imnzhcxg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2xiuykdwz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2khefahwc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2friztdla.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2yomfunar.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2isqyhcfq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2yiqeqznu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2rzfjizcu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2osxrvqhz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jsislmlb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pandkndf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2oywzjfvm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2atfjiogo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2qdhrriha.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2eompwknh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2egjtmypu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2sslwqtlt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2hxcuavzk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2llnswwpk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rxdrlnyw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ejewrurs.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2rnkpljdk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qccmlaym.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2msguxlpq.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2bspclnkv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2dzkmqcsx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2wagbqcwy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2egzcxuni.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xwjxjnjh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2tsfsddwo.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ktpfqine.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2xqvixczl.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wtoqthql.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2thzbkfre.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2fyioltsq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2omwcnoij.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2rnlnchxl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2jdcuzhek.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ocuhiovo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2nwxphcqz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2dqevwbhp.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2uxtyvcmj.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ezaanauo.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ijsylrwq.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2fgmppcvz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2wixlmqtq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2jedfbtgx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2cutmmngl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2kjxeoxvn.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2mvjdiqnr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ssdqrzkh.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2yezuoqhe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vjasyobd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bxxpkbde.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2wcjeaqcj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqvskbjw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mfnstbuw.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2hipsnehv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2lcossbmv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2uslsztgr.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2udxgomdj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ilwgtese.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2enstskvb.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2udbvamjz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngslugrg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2huklfumk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ujdvsvkj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lqjsxdst.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2gtnjukin.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2xhfhcasm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2qbbvxvgg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2azjiwhij.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlzjvhct.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpkyykvf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vsqkiyha.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tlvsbkln.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ymzlifie.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2hlxxjcqj.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2kibrlwkc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2wmdxnokl.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2xbcqrkza.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2milmaoag.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2jzqhxqbt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffzikwmi.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ujkxaqaa.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2zesotdtd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2qilitvpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2efabvnez.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2phxbmmxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2snqejhij.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tepdnpyu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2erjhvfsa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rlrwhavl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2dgsfcoga.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2nwaptwiv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2dikhcgje.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2hrvyhozr.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2cnzssbtc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2pxhhgwzu.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2qctyibsx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ywxqusxa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ayjqpqec.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mvlbkflr.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mzkdpocm.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2soskbmax.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qpqwmmep.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2lrcwkrzd.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2gfovolwj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xchehpoe.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iuvsdcif.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2uspmpdqe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2axubpwol.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2uacqrdav.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gxbgsqcb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wjrmhiqm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2dnchyqwf.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lqucdovn.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2maniupke.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ycdybddy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2etghxbjg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2vpcqcwuh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vefjwtxv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dmgvkunw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2cbbwbbhk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vddmxcvy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2bdgprjxj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2pniknkqt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vcauwgyy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ygrqadpw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wurelioc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2jhuooiuu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2hdtaatkv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xaitiheb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hwdmadll.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tqbtzenj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2glvjzync.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ulovsqwg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2czchvmza.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2lgujzocm.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qbcoyqyi.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2rracjxxi.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2atthvclp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2edxvrtet.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2czqddjdf.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2gzxzujrd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2wprhvgwj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ndyhxalx.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2uapgdtyg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rjjulxvl.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2frxkrold.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2mbltaued.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2teihsrgs.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rwfwsojj.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2upyofkfe.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2hlydfcis.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ydgiivjn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2tnsvzzst.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2kfwqjumb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vmcizaaf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2rpskdrar.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gerwvexq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dbiznqpt.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2siqddwwo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jrmihwwh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eitjxmxm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2agzcwzhy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2yiyxbuze.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2zjlahpvh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2pmyxmiup.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2fxdkaxno.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2iouebsrk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2oldaprqz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rnoxjvjd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2spuxqdyx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lbgequcm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lghdevwl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2rittuloz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2dwrmrylw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2bolmiydq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2vbxzjsve.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2oxnsyvch.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2raexqags.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lzccjcuu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2jklgchnn.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ykiosyuj.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2okofytyk.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2sdpjgugz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ukkmblxv.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2rqwepklo.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2fplodomt.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2wlofjtbt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qysjfmak.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kxpzqugj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2efweoqsx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2lgozakyl.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jtgbmhty.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2epgdbscb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2duimwpht.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2mzpatxnd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2bwccxljf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2pxwgnknf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ebxvimmf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2vjjmzfoi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2olzuhhbh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2xeezwlon.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2xkscnpqb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xfhldcek.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2eqummtwq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2spupytnx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fgqivswu.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vbjreiwn.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2uffkupov.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2fmhesglk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2fgjnqyqm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kofbpnkh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2andfqmpu.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2shzeplld.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ciuzaphr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fsbahmmf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fesinhwg.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qjtxfltv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2atyxcvcu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ieacqweq.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2fizpjmup.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qrprccbf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2whwmtdau.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aticvpyf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2sqlfgprd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2pagwznii.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2evidpyqb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2lphhjkzz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ksplmkdt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ouyvzpcj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2lcmktbsr.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2bogdgpkf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2buiymrje.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nznmoruw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2mgxftczq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2prukiazr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lbfwvdsy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mqdvfcdp.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ufxluqvl.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2bsqugfvd.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2yntxfjrj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2nfotgkxf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2plspheei.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2cgmsbruu.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ebiasbnj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2hqnanmtq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2tumhkwmw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2pikyuazo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bgpvfftg.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2zaqketkd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ydfplqfk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2xxeqgusp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2qumiyzzo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2dmkguqfd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2vgwgaomo.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2uywgseam.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2twjpfohc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2sdjggdni.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vbpzjeav.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2lbaplvwb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2czailvdr.html


<!-- 参考信息 -->