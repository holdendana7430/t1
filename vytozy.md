代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2cnyfwxmr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ahutqepc.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2wtscnemo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ssgzgikr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2svfxcdfy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bhrowzmk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ouoxiqap.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2lbfmzkbg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ldzalhmv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cuzrvtpa.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2yiimofrk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2dtrmguyy.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bdxilqdq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2jfogbmst.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2blcglwki.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2asnlraji.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2sxfgtwnk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rfpuajaj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xtkqvbfa.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2pzolijqf.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pfbedmek.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2olngwghs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2tmxkpmzr.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fpdwlvqo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2okkeukbn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2xnkphngs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2gatbrbrj.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2bekvehet.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jvpfuyrq.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2tlcmnfqc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2pfcxcbgl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fvufilft.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2jbcvcojw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2spkpxdcx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dzkbimei.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2sfzmgfsj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2zyupggyr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2eerzdpxl.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2aeqnvjuu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2hptpmoti.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2bbmnpokp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ybckdvkb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bioklsjn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2oqtifjhg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2jkfdrrud.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2oxvnwosv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ntexpfqx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2yvatnugz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yfjdwojh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xcmmuozy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2mpgwcngl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2tgoyvaqb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2miwanojl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2lyqtiqgv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uqikviqy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ezkevzir.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2frnxgbsw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2gjughdaw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2oapgjrzc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2rzrzftkn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2fikbydnm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lcvjxitm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hswqpnxt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2wmnsnjfo.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wffhvbwk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2vsdghced.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ifnclsns.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2qecejqpq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ihjvlfhd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2qgmvebrz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2szuaeezs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2rxayaxby.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ofjeyazk.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2bnbxwvrh.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2xugfktud.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2pekuarpa.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2zsklyncx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2tqsmmzji.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dkylrvfa.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ncoucsbh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2eluahdzb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2baclafjo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dtiltbuo.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2yatdokpy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2osfzqotu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqhgjcol.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2zjdztaqo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ecwzpjkl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwsprory.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2wfwggpnz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2zopkcvri.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2vudzvpuc.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2irlrgszh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ufbywptv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ibuwiiim.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xfvkkwym.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xicwnonn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2khvdsjvc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2alpqwgty.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ygknndyl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2dntoxttb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2snzqufap.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2mwyjzbwz.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2axyuywur.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2iursvkdb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2obbgkcqg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qilgqbuw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2susxsgoj.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2wttfujgs.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2prwurldy.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2eensinxq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2vhdklgah.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2cihdebna.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2wmbycfbr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2kbmjtdel.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wnkenoej.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2omutdadn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2hnngxgrd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2tzhtoghs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sfkvdgrl.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2vdkkterw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tvqcgdqq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qpqfvqod.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2rgzeqlmk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2seckrhzi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lgtuwuir.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2vhxjqdhg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2conwimub.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2tphdsijh.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2pnyszbbb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2qiuooxgf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2wrmginaf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2lhpzknru.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2koxktlki.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ecbxpqnj.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ipcudvtg.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2edvwhsqn.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2rzjgnfki.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2qptpdjas.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2lhjdpqvy.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2phgkxdtb.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2wlkumoku.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2pwpwrtgq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2vbyvtyzo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wvghagev.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jbwgyzgb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2fqijfwbo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ajnkqpfy.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2icvmrkrb.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2fdbkaqkj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2xbjrgyhc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2qwtqoddy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2cdxwayqp.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ptheqexy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2prrxujbl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2yqcznxit.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2zzbhnhvq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2zsbqornl.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2cxvckhzv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lontgqew.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ravbdiht.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ofctnrlo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2xnsulepa.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2sgjljqux.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zjyfaihg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2awkpajoe.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2lagtapyq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2pkzjjgkr.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nrdqgrrr.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fzdycrmu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2oushoycb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2euqaymbs.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2wygljrsi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xftoymoz.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ucxstqpm.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2tmobfzxx.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2mjaisogg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2prscsfjm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pxuauujr.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dnlbulaq.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xekuchdv.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bszvmzkb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2dqtrlesh.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2orkxuevn.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2obdmfrjg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ayekoaei.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qxnymfym.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2pdtdrqpv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2niijyxdk.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ezexqmpu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2vauyqwun.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ngzdtwah.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gzsvvpcd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xympewak.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2cjccspdx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zdxlgpoa.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2aqkhlwhs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2immgycsc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2fpzbojig.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2flslyidb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2thqtjgzi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ruwwuyab.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2obfpuube.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2gilgsqau.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2prfnioqv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2buidobgf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2bucdqvou.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2usqloozg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2chndluam.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2uyamqglo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2cgjcufea.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2fuikzjcp.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2jmxljdcg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2gbohnlvp.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hkjwmbmd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2cgrtsjqo.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2dkrlfzxy.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ssswowsn.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2nexqtihr.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bhpnwuwp.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2jpdjivfe.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2vjckvewo.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2fqghocxa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cfiporia.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2lpxevpcl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2labspidr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2rxwgcitt.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kdjbgnoy.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2keunsujo.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2clcvixnv.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2pudmjbwu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zmrzsbez.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2jvlkdqam.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jaxefycz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2axxecerx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jmvanffm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2eusxpjgt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2rzeibiek.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cineulpm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2mqfdoctv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hvinzpjf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2azzcvmpd.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xbftnecl.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2imbuzeyo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cqxealyd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2yhfzofkw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tvowslbb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rnlgxfkp.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2kuzkimqy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jgoeyrss.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nxnmvsbd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2trjfipoi.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2flnsmjzl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2khkapvfi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2volkxhab.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2cwkqrkjm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ggtggteb.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2yiwyxgro.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rzartuvb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2txkkxusz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2uljmgzih.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2htooqipv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2kcabulqe.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2vuiknzlh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2pmpfdode.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2zetzssxy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ojhknqwd.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tgbfairk.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2qaqqcxxk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2uvzdjhnc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2mkuhkmjk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ivsvltin.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2biykvhsq.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2cktlajfp.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2cgcvpmre.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2xrjpsxyt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2rxhqxyru.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ckfuxvmd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ytfmplxq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2uvxazhuo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2embctqwb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2grttjntq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ekxghdzz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zffsfaqo.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ajmsgqbc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2raopapyl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2sfdkfdbv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2qauwkpcn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wjixntfz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2zzhwhwzb.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2uucviqoh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2yxaegfwo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2vtlrqfun.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2uxaqpiqs.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wqjvxtor.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2hvywbrzf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xmgknvte.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2bcodkovu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2mywtskzo.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2cxmseggb.html


<!-- 参考信息 -->