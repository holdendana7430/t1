代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2npaczpgt.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ezqwdcrs.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2sanusvfd.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2wgiwegnl.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2brpkoujp.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2rppqvjsw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2aptnmqfk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kiergsha.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2fwtcgmyw.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2izrsumay.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2bgpwluqp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2kdtvqxzj.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2cdpeegbb.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ocucpgdk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2kvtrhfes.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ebtnnrqa.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xhlwbwoj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2jhygahfn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ltikulhg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2abibivkh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rokivfgm.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2fcmfovyw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2toxcbgkb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qxsatvjf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2utzteata.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2cnoczaht.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2gncunvld.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ymkxzfyi.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2vogjkbvg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2hwwrqfxi.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2avbhajsm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2wgauvybu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2lnkblmri.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bzcyqgan.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xxirxvds.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2zmgswtll.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2dfwwxune.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2igklfeyx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ylrqzpum.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2mxlfvoqn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2fcfislxl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2moyfovlt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dipzvjiq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ohsjeitc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2gabyeqsl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2wwcvswdz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xddcwhbh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mljwyvqc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2hswiesdr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2gmpkmrea.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2fwapriky.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2bfpokadw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2kcgrxzvq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wcgxvgkw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dflhygyn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2tawhhtkr.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jgpeuqec.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2rkbjyfab.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2kzxzzllw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2meaxxxnp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2uahpnnho.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2svxflzhi.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2kggvwrnk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2tvifwkux.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2fyrzkjpk.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2jkkoslus.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2pdechfvp.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2zqvyleoo.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2sxmugzzb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2gpepwszt.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vdfmvglj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ltmkbpsn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2dsgmuyce.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2vruntnfu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ypnvjvnn.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2wlsuwhwi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2oqblbqcp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xzoujfnu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2okniactc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xllzrjgq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cnxemyxc.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2lahyrwfj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2urpvgbfg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2svhxqqzh.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2dsgvnwhf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2hbznxnkq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cgsctlmo.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2uuqultbi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2evgrqfzg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mdxenqqt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ppqerpal.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ocktbmvh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2uecrlxpb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2qtpnrxqr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2gcinbsnf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zryamhuk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dmqtitqy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2djgqjdvo.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vuzrxrql.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ahghwaqo.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2yeyxgyzc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2exnaflum.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2xqrpdckh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jlkxtvvr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ipnpolkk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2lrcelnft.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2wzhxalms.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2lnhanqhh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2zkqqsijp.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ynvhectm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2plmuxmym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2igdrgvnj.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2vugmqorj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ngmfcoza.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2uwratnho.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2mxswgjrn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2fctcsutl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xronzbrh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2fmlongwp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2yhzhrqbp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ubovcjzb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2prjvvmag.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2xjgfjmyi.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2whbeenqf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2eacuaxwy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2azfujium.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dlzkzexl.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kuthmdly.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2hfpzedak.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2rticakue.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ogjmpxdo.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2thfdidaj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2hzlcvrhd.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2akcgkxbx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ermowdsi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ragdtpxx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vcoytvwb.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zkbcrmth.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ckykwsuf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2pxghscrk.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rgrrvrhq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2pqgnnclj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2unwccrls.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dctejkxw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2zdhuqtpo.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2pkawomuo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2csyrlkjr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2vatnahiw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2hcegtguw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2wbldkgnh.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2eznazyld.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2syxrfomm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2erissxzz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vguhrcvb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2hxmvioex.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2qrmticnl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lmonbwhw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qogdubxd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ulpfimfq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2rkgbvtre.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qajxpsfk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2aloehzkw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2basilqvd.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2odebdljl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2wvgziboi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lchvtjcf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2slhvoclg.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2lnapeiwv.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2kyaavwny.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ksndooqe.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2buqytjrm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2juojrciv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2sgosfegi.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ehylorqb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2yiwasajd.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gzojqwhp.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jezsinuh.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2plwspdsg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2qrashrxz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2jntkimmi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2fxfvtdas.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2dfnoegdg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2hqbyzkoo.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2wpykeref.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2wqurpuul.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mulytsfo.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2lbkllmkg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wrertvyi.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2oicvvogb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2gqonrias.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2uibprowq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2unhksthc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dlngqdrh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2iapmwsgd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2uerjpvbx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2zyzfehbd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ueccuudt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cpksorzr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2eukukkxx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2oingadhv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2bitnxdxr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2rnluhrij.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2eglitbln.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2pabtzuqc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2vcrhfsxo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2jwxwxltr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iiufltqv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2vgchmzyy.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tmtcswmj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2afbbcetg.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2caqselxa.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zephjlzz.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2jzqtqpru.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2othltxvx.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2bmauiraz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rquwlnls.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hrszvdqj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ajbfnzho.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ggbiguio.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2axmtavev.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ffqutykg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ncjjzbib.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2mbulzfhv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2rrchwitd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2vlomnpmx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2dtzhxoxn.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vqijibjh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xzijkslx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2lxhvrmbj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2mtbabkvr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yrnahwzs.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ltpuaiqj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2tpadjrvc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2losugggr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ewweouds.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yagreegk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qzkatcsn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2rthapcti.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2imbywfmm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tonsrvch.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2dxfppunt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qumhxxcv.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vdaidzxo.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hmxwxdop.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2excqmwew.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2vmmtklma.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2fzzfhons.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2wvalawvz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ddufgkzr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2yrfrmbrj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ciquxgbj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qhxrlqsk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2txppglij.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jxzdqdbl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2qbryrzyr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2kwqhuclx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2uyshynes.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2eicgjvhj.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ubbxcgnk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2hzholfty.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jttnykjt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cabhesyv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2zhjoikhl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2cacntjkw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jeuhrlxn.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2dxzjddyn.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2bphuwwkq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2msibcqzo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2xbksjekc.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2tsczqsjy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2rterfoex.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2blwckunl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zuamlcvw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2eklzgjqm.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2pisbtaub.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nqldgixc.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ujhrzqdo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2lavcdiyt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2mgtktfvp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2yiycdqcb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2kwnujhaw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2wdcyiygh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2wwatvbne.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2yqshlesp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ddkghvui.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2fzlmvrgr.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2aqipbzxf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ovlldxde.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wokjtfpo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dgpgpzef.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ttvwfkwn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2izbgiahs.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2wlupdnky.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2cyxvftyo.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2inwjxvin.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2flvwbrjt.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2tmiibehe.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ijvpkkan.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2amgbyadb.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ccfwvdpc.html


<!-- 参考信息 -->