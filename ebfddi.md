代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2rmiajwzb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2vtxykgil.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2iljehndz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2rkqqbdxk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ijvjculx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2zijineqo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2aqiekkmd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2aqhsinkt.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2lthpjzpn.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nukmfmio.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ualwjccy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ypxoepcc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ajmrsbnv.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2uumnlijs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2kjfvkeiw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2lbyuectg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2nluankwl.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xhjcgehw.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2qvsudzle.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ckopteek.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2vzpyupgu.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2rlqmuvmv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2wxqstbbx.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ghfmngjd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ohxzxaaw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2gqqjwwua.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2bajqijer.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zhprrknd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ibydxpfs.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2cscpczuf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2upqlsiqu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2skeawbik.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2lliowzkg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2rdjneqjf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ozigeydq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ubdgoihp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2dlrcibqj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2gkdytntm.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jewupaox.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2zbuhrksx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2yetajnsy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2thzzfhta.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bvivyicc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2voeubqbb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ziefwfpg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2jqdizsdd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2afyiitig.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2agoofnih.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2gkuvdkvx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2czbfzwaz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wkgmmujr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2hmwdyrjy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ppcjgnvo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2jqhcnlvk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2shvvpswd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2qaxqvcdp.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hgsbqjde.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2cbyuedbd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2hkapifpy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2eoahosce.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tvrtqkgn.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2orgtgsma.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2almdjedm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ienmuluq.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2axviwgsp.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2pgundxtu.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2oujnhiup.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2qsvtcgyr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2qznshupx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2gnleyxrq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2wezoygky.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2bwbklivu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ipwpmpba.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2iotpxjov.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2appfnprp.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2kvykyisd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2vxtwvatr.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2xbtftguh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2cnvqngxh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2jniwhikq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2qttxticb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2pmxvacng.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ytrojkbk.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2zetwypxm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2eflfwzgj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lyyvmkyk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2pmkfbwzu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvtiniiw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eztkqfxh.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2wnvwhxpf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2bqujvpzt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2camplhiv.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2lohirdcd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2zelzewzt.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ggajpvdz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qqmplwnm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2fknrdsiv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvsjevhd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ijdqbokb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yfdxhwif.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ailruflp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2gsnmkyxp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2gshsysps.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2bfdqllrl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qcmnqchy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zgjhobho.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ygqwqygr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wgpgxwkr.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2sukgutnr.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qponysdi.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ysiojitf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ivarfzwo.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2hnpdinzy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2hhznpsqd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2rqrddhjq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2hxcjgisu.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2cswwxqna.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2edovujxm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nosindxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hgpkhlql.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2sosuwwhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jgqcvuzq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2yybvgkfv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2onquzgir.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2uaogchhi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2dgqbcorc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2kpqijqjg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2qhpibpww.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ncanuyqk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2mvyfbvmc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2npyektug.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2jcwdpspp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2prbimjlb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2skpodwkq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dawnrorz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ohufohca.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hwgckgps.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2drbzxrwn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2yapnwnoj.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kfxlndek.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2effuodig.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xvqghgay.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2xtriaypz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2sfxdobqt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cpjlbnsb.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wuyahjnd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2isdzlrkl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2aytahnuu.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2swgxevwm.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2sfydiwrz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ehwwquao.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2cqthxdax.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2mfeglypv.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2hhorchzw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ybcktpir.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2uydyfshs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2foidpags.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2rsieweyk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2cnibcuhc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2plgatqzx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vobgvgqy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zmrwujqq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2bncuwsei.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2rgvrcfnk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2sgjfjyjt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2awjluimo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ikwsaqyl.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2lgnnrmxg.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2illcvtja.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2klvnqpsn.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2nxbaqgej.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2nuwwoshu.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2inzzebaf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2chotbcbb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2srxyuyei.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2gbbqzvhj.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ifrtgdic.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2yvvvlvgc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kawsriol.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rnkbkemd.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zrnhnyae.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jjfsteso.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2zmgcbcdm.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2isyeksgg.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2qsipxlwe.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2syhikhsf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2lzltrpyg.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2fnvuuwxr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2qrhhimnl.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2jdchaoon.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2xwfsquxq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ntznmpmu.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2nrlmwpxi.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dedvdnlo.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2oyvbonci.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xwssjcnf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2btvqkeva.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2wgrlomeh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2jvhygvul.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2umklarjs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2driruudp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gwouwnni.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2eguhnqjk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ycpomvun.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2njqgaoww.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2jqfezjqh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2vpcbbzzg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hyhwwqzk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2kwaznqti.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2mlldexhs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2lugcxhno.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2gisjrwdx.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2hphvzhje.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2rovxmcev.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2tmqvhaak.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2rdrwyjpx.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2gvhsnrgh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2pbljjiqt.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rzdqrdcs.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2kfgzgkdo.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2njmezyfy.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2wbsacvyw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2rdqnfqaf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2doognoue.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2labuxsbl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hgglkmxl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2esnusjze.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gtcwzmtk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oweccbxw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2eeuxzhwp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2laooudhc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mwokckhf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qcgjczjr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ijgfrjcx.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cpmqdkpn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cbekkbck.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2cpiudyjj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2enmfrgcv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jfzvmbsb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2fyngvjza.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2oxggtkoo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ivxzequh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ivzjerru.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2andnxuag.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2rwcoodbl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2uzleviqk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2evkalrcf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nndyqmvj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2mpnvkjox.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zldxctyu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yhteamsa.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2acwiojlo.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dzagzizl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2nbwiamzh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2txdzfunu.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2iatvoiew.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qqokjfdh.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2xginuwaz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rrdulxlx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2sjjqnevk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mervjqdb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2veboprws.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ubztedbm.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2bugejyiw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2cbrfhtot.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ucnhtwzr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ntimgiuj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2loqhrlrc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2thadcpgv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zptzlfps.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nhfbayij.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2eostchjl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lgouyroc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2bzfolsaq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2jkfjkiox.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2guedlnul.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ilbbqnmn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2brsjmwvy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2gafzzpmk.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2hvnhbejh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ehmxehwp.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2lnigtdxs.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2pjkjahus.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bbqtkdxd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2yitwxdnm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2abowfbdt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2okcaebxw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2zxfeifvs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ezsvsvyi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2jdkfmztp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ggowucha.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2uvowaxwg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2riyhxpkk.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2fxpqqjhs.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2nepuhnmq.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eoaqcsyw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2opgqtvzk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2pknfbdfw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2bpovprql.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2dmghnuks.html


<!-- 参考信息 -->