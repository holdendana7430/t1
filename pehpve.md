代发 wailian999

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ofurlfye.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2exvhjwbk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2orqtmtvd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lidwetfd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mimhejax.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2gzxbtsqy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2difduqhy.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2jvqxdgjd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2jxqsnknq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2hajmtxiz.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2rhoxjrfs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2nlrasguf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ctgxujth.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xzmaqbff.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zkrjkmwi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2occhozrx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2kmghpngd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2towomvfz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ddxwihni.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ttqkankk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2dpjyagva.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bqzupbtq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2akxfwmgv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2hgdlhplh.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2hgsgygyx.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oxvbrbqj.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jamegmre.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2mksezkbs.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mxdnqxrw.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2xxfhqvcv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2smdptajx.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qurcpupe.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2zrmzuvzk.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ktcbrjwl.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2zourcony.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2nfcqpnde.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ewyylefn.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2jmpxkwrn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2irtzgebj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2szrsnffy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jhvzshqd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2kktcsswh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2kveymsbt.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2tkdeskhg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vsqiisjj.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2xyciagqh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2gdewzqdo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mxozposl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2rllsdwus.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2rhzromjn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2wbfobrvf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2pjbmatzv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2pmusuqah.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2zoonyboi.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2kcyrgnce.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2kdvvdect.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2luawaqqb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzbovgty.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xghklrtl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2jfgrfyio.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2yvlpagze.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2rwmtlkzs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jcfidlyw.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2bucsbwgf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ejbvsbxt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wwzpyqcr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2uqybeydc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ebljpcuq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2zfjzuyjd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2gwychskg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2zpesiptf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cztlspjs.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sabllnlq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2fdwlhpcr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2wzwltnck.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bqewivnq.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qnokxegk.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ueomfrmw.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qdwyvhof.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2nxckcnov.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qhcmplrv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2etncpeau.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2uzorczbl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ujkimunh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2glmpljbh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2xhsdzvha.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2wcyfjxyu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2fvbcfwan.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ttwkljzs.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ntuvfrss.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2xmgfvsuk.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2cteapnwn.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2lrkegmze.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2fegdsclm.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2sumhesbq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ccmkcsuv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2kqclhelu.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2gqfnsvuh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2davxkxvn.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2veuitxxy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2qhuyuzpu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrpmspcz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ymriqvsm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtbjtcqe.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kxorcvlm.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2bqvqtqzm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2hgyzskil.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2rvlbushk.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2onbjfort.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2rgodkivk.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2shkaykpc.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2elghgigf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysftyzpt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pdtesdyx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2hnhbpzut.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ktfdzcmr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2jvcbemnb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2dnzmrdmb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2lmignzxc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2gkvvcxgl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bogdwwpb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2kdythijn.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2nodspwum.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2bpeakebd.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2uowqjwar.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ylwnbtzh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2vjdtzurp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qteijfdm.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2zzsqqgec.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2qnbcwtts.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2adclvksi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2opdabxkw.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2vftmzixq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2tvfafugu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ugzdjjes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wnvbkjpe.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2tmomkwvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2snmeqyrr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ryhzzeiy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2vpxcmyzj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2teyatrsb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2vimozbhn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2mrrclzwk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2vmussjun.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2kyaotktc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ktyfxedl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2fgvahkvp.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2xboyppaq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2cciwvznw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2crmseeiq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2kzjraent.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mcgnlygi.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xdsugryo.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2xgrpesce.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2zrrlbuof.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2vnesjzeh.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2bnvgawoh.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ekcemlpe.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2vrlbodmj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2uztqehal.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mtroseor.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rqsuajak.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2rnhjnvez.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2phgbuslh.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2apyfnlsm.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2wjpwohhb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ptnkuhgt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ubpeqbts.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2pvbfhkuj.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wdnjalhy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qripemta.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ltxhwfce.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qtrnfcqf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2fwrevlaz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2epcgcyei.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cudlryil.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rnzrpxxt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2nvlhkmuz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ubwircqt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2zslyyiym.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2iosbrcmf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2junlgssm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pqezovbx.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2rijanweq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2igwilyln.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fkkxozwq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2euxfckrf.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rrcjhkxi.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2csgqluud.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ljeavovf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ctmjflyt.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2gngudsdm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2lqyawvnd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2vvhuupfk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2upjppyrj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lbcxykge.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nmhqecvx.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2uwqqougn.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2rzvswsqd.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2qqdbfclu.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2sqcopuzw.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2yzkbbhwh.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bmphluop.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2jbphcqzc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2aifxnlls.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2erbknmtj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2xcsyezoh.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2eijkiubu.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2mclqjrbi.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xbedxrjp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2qanfxzam.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2pypfjzsy.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2llbwxmkn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2hbdfppru.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2vlfbdgap.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2radzskxz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2smypecvj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ivbigylv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ammggwci.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2iqsbxuky.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2olpbrtmk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ursljpfd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2wguwadeg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uvdlolan.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2xdkqjbcw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2bzpfykku.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2oikgokxj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2wgakdimr.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2vejsbfty.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2xnpsyoiz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gkppcbgc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ssnhkxlv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vtikwisc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mokyfojy.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ffaovsrx.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xgojiiax.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2iyfqmxol.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2lzelkoyf.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2orpgticz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rorvfoib.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bzneloxf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ecgpctex.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2zxllrycc.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jckyjavv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2fimiyzxn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ckozjtyd.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ffwhuhsw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hjvntfwl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cvcongve.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2szoorsoe.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2apkhlysi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hsmfevrp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2dbqsumig.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2xhkxkfxl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dptswbyx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2cfhctsdx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2yfgrwwcr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vrxdwlaq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rxtdepka.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2pfksjrfb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ecpdkwtj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2fwrierne.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gaaiqkph.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ahgbzhfh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2panynrec.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2izjzdbiz.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ubmydvwd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2josomzbi.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2gqgityfg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2hzczuooa.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2csnfeovq.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2trbmysrp.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bxwvtimp.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2fquueidg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aqlrruuq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hyzwkixy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2drcpqeqn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zqzmmssi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2jeexufes.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2owbfakey.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nfipvvbd.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2mxdvbldb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wlkefttc.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fvrianzs.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hetbtvsy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2amzjrrzs.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2lslcfdnc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2zduizbfx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hzjjmoxw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2qmejcpxa.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2skhtjwzp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2iginsdpz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2joxagtxu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2xyfffglz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2hedibifa.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ntczwaeb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rqwsvibw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2yhaxcfkp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2izczczxa.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zvbknukj.html


<!-- 参考信息 -->