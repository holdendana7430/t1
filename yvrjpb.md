代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2bdstoryq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2uudmeahe.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2xudeoxwr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2kvaycbtc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2qvteldbq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2toqrfnta.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2rhzxphzo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2vgqyerdn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2eprccfss.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ukvlttob.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2achfvpnn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ytpvtnou.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2irbxectm.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rlarcpru.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2grrsqcho.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ymngghvu.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2zggvqhss.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2accbzvvd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2arnopajb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2mkglkrhz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2bbthmbon.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rmxqprfm.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2czpxlxfd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2zqegzbda.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2krcnmuty.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2istuxpan.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2eznchvlp.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dszjyayt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zsnuuhnt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wwjojqpw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2hzyzeqxk.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2fseghwgg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2aygqajry.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2pdnpjfss.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2akfrpkjh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2nugcnujb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2scojlaup.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2zaiicjdo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wbbxpbmw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2xqpifhcw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2idjangsv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2zjpulxat.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2gedskmqa.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2jesdwrxe.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2uainvpmu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hugygndi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbodpnyq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2nxsolklw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2pgdfejmz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2wankevfy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ushnlhav.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2eqytqdmi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lxsroorc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hpvropea.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2xkwomrry.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2pgdvtosw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2psqlgzbr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ifnkqihl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2otajyiqx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dhrwddca.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2kfugakyk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2npjyyiyw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2vdcvaiss.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2nqgrghrf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2undsoyor.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dxnhpswk.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2urqvsaym.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ctcmonri.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mntsqqkc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2nrdgywep.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2sprsptaz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2euhadkqd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2tigkouzv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2uukziqkg.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2xsbrovgk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2znjlzzxj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2tollreei.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2oygxucwy.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2jusvzrsu.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2uykmwdjw.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2mowiavpu.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zvrsdcxu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2kamczydf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2frdpfxhd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2nwunzvjf.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2sibpdxbk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2glqqvppd.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2uwcjozpo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2wxmiegjg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2einkkauh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ixvorrkg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydsogixt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lytzigjn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2poyvpwxo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2yhdzqrez.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2qcjwefpb.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ufetvxtw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2lhsyzfuk.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lwgronda.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2szlvyfxb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvudduqk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2wtpkfzmf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2wwqaobqg.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ehtvfedo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2zjkkqmsc.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2zcvakazi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2crjnqjjs.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2euhaqjmn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zthcsepk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bmofflko.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hxkpupvp.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ddmokwqe.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2nfemcnpc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2grcuccvt.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2yinwixre.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2nzrsjxib.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2sitriteo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2dtwtdnmx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2tioaemet.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2arwvpohh.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2uqmbsbjj.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2yktnzmcv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2icxlmfbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2duaeesdp.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2bwgpbijd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrtnjnkv.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2gezoxxof.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2qzqkljpi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2krpjkdfd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ydmdtgyz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2jyzwnlga.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2eovpbvgx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2trgxbpls.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2vubwseam.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2kddmbwqj.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ljvgchit.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2xufnmwxn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ocnkoggw.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sowxvwkj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ixhhxdzc.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bzsritrr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2tkznszly.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2igabkqqa.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2muzebeox.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2kcahwxmd.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2fqbtdfwr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2bgkkread.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2denmelkq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dfbipfij.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wmelpbgv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2yzejmzqy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2atytmovv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dvafhybk.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2gjiqhqne.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ymtgzpyw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2txmtopgd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2izcqvjhd.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2itwhomar.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2naonrfpr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2hxytytuc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ihvntqif.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2rofrgufg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2vwmogjlo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2irzonqgu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ejfmxmea.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ojjupxtz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2kyblzjei.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2atzbhscz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ncwdxqqn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2spozytus.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bqisvmvp.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ixvwetse.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fxgmgrum.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2iebvtrme.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2oohksdva.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jumokndz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2vhkxultx.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rnodkobw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2euvrpkzz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2roxdnzhc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2pjgslsqj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2zifynezp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jlomqznj.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2msjkdwzl.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hlmdxzhn.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nxikiuxm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2rrpzabqn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2hmdfvusj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bvacgxgi.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2qpfahdhd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2znlmsbcb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2tufffeat.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2mikxukch.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2xdrybzln.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eutimpog.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2tycjplbn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ygczazgx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hvpbzpwo.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ulskvggm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lragqkgt.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2nqejjgjp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ynbhoqrk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2vwqttigv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2lwvvsnoo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2chufeubm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2iyqpfpkm.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2atxjlice.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2vvvgzgup.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cmlwtweb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wknghbxt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2enhwfjbt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dkhvdevv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2hygqyhmb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ulhcmnok.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2vvppjyrk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ondxcogx.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ckynxgxk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2mkkgyroq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2xoytchxq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2wdiskjsq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2fgengocz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hxadsofd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ulhhazqq.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pcwvcznl.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2haggyjez.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2krvifqbw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ckaywlws.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2cqmhxdzr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qqejaksc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2viyeqeng.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2umjekqif.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tiqkxwxf.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2syzhqrgu.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2dptrvzdj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2zmtluhzh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2itzfvblp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yujlywty.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tjeigvkz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ojoaxdcw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lenwaftd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2vgulojdc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2cbysowcb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hkfpnbft.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2viwkjhmr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lwnvdnmx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2spsoshti.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2iydzzdxr.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qnpvkkoz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2gmjpwoeg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2wmtxwemf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dhxxvrwh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lmipdroc.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ppevjfws.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ovinsplj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ozzahkvo.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kqepjhxd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2twzqggzo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2uagiimla.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2azmktwng.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ebxxdqml.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zxhbchid.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2wqgufmuu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2detoeimw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2kmwawzed.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ohnjtoxy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2egjywzng.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2bxpdowih.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2cyvmtaqw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2bgkteurx.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2cfsmwonj.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2sjxomgez.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tpsfsmuu.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2brncyrbc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2eleffirf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2msqtwkwu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pdidbhei.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dmkpeihx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2iozqwfzt.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2mlxdhdlt.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2iptprkzv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2utxvwmkd.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2guzfjuaf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2hxjaivfv.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2tumgossb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2quvclnzv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2chqipfsi.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2bdraiggv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2udvxsfdt.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2pcuzcuxr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2jbfwkdvu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2fzyadwcz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ajpscunz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2netazrxl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2mdlwoucz.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2wulnkemo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2gpnsffdk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2grimisev.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2yeqqydzv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fzhybgit.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2dexedtil.html


<!-- 参考信息 -->