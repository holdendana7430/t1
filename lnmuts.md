代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ghwdaaks.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yrerfgjg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2juuysdpm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2rdraqhfr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2tlsgzubz.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uxksegyt.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2avcoqhlk.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2iinwkogd.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2rhinxipe.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2qnhoiers.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2drvxhziu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2tydcjcio.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2xzckjyuj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ntcwqnse.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fczadzgx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2dijeycec.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vclriypz.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2grvbaqao.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2vwujwohi.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mkajrymd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bbxfeikt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2wywmyyai.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2irjkxnlk.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2flthfizx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tslknoeb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2cabmcuie.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2lpnzbywn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2owvfoawp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2vdgtoklk.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2irldszsy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2skntoaim.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2oerocszp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ifkdjooj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2wvclmmpv.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2exlluxnt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2cbbzhzts.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2krimqnqn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ysslnbpb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xnqfakhs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2rwsbtvoo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2uethnpqu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2fntlfajs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bymitawr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2bfymmjpp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2raaqmuoj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2czqobnbt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rotmqkqn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pboyrtpl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2oyereads.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2lxbzqxbr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yrxgnejv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ebwjhspk.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2afykohak.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2zmuwufsu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2canfjzpz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ouwbwzha.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2gjdbygld.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qmgjphpr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uoifgnxr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2pwbbomtb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2bbpeqxfr.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2kzrsjvsz.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ljrjkbpk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ukeunoko.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2auvigmfj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2jjawbryo.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2pltemyzb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2rxvwgbpd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2uokedyua.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2hwungdzb.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2yyyyxssl.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2wnxufedz.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2bnjufjeu.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fbrrfxfj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2swmzuumx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2sfbtxfzl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2sbfzzfym.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2luzqeqrv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2thzzelpk.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2cmtwkjkm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2orzihkwl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxeuqrta.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2pwzxdhfn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uaarvpoi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mswzzejv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2izxeofgd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ywvdfexc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2cutazanj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ycwzfzkw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2witprjte.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cjtpvetg.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dykdvnpy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2kiqnkxji.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pytvrkmj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2isdgmeuj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2erhtqnix.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2sutwsapk.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2zutmutnc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2moxlaxjy.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2gwjplbqf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ybyhjrbg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oefthqnp.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2qltrmicx.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2dagxvjsh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2nogrcgnw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2aclxtgbt.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2okrgheud.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2vuxzxzup.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2wabggjpm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2utwapcrb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2cncgsxcf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwchomby.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2xyqjomtd.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ieieeqxw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2qavlmaqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kkwyfjfy.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2opwnecnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gzsumwpb.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fghwlxfs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2rutabxel.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ezlofulm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2kcsfgpcx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2rbnqlskw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2kkjijupi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2furblila.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2bzigkvye.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2uweyvmyg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2xuuvvbsn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2dhxgbvuh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2mtlmufzo.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ggnewfwb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gdefvdhj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2sxzyvzcs.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qxwqittx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2bzlgvdyo.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2jagsydzz.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2tqnybiyw.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yulrtpeg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2gdcrtegn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2phzjrtmw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ttrwpxfo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ncgusfwx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2gdykysgz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2fotieknj.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zrniatzb.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2vdwihibi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dtlnwfsa.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rujmqjwn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2tfzgsktk.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2qdpdhghl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2muqymgog.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2rbuobavn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qoohdiig.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2wcwptkna.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2zqpsksld.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ykvhtrvl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ekzwkqaf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2iwsydykv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2zxpvthqz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2weasglnk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vwtdcqwm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qyrrqwfp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yrkoxrzr.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2lmrztzyl.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zrlozqdf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qtvwuuji.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qwparqsw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2qotmfnye.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2qkzrcgcl.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eozhcasz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rxzuyrad.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ploeblvz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2rckaixtt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2cnrzgulb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2gxgkqvwe.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ymeoxfla.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2agkvgeae.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xvjdbqhv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2kuyudamt.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2didigjyx.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ugavxnvv.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2isnywqgb.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2zllpksjg.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2lmrzbaon.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2eoylnyvf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2tdmteoty.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2oqnspsuv.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2dwwsfmnw.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2avdsldkl.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2grvdxhzz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2isyieete.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2audkfoma.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2djsnnlmo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2dksjxoam.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2tvbmsrkt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2lgafgetm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xmpcxqyn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2golidgge.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2vxhmfyob.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2kjvnasyr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qyxgspcg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wezffhny.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2upsoiigj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2fwpgcalf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2slgctfnw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2gsefyvlg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2oreybdjw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2nghupdsl.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2vgffaqhf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2znlcehbc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2fhpjqwgi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2lxpnypnh.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2gdhbfkdz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ubjilafl.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2mgoyezxj.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2zsryswkb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ggqzduso.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2iehopfsj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xsxbpekt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bvtscejv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2pgmcidic.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nuldvdgj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ojcejomn.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ydrvkjhq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ycxdvhfi.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2vksovckf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2hftvkcbd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2hrbwbgjz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2cthelpzi.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yaoagpzl.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zdetarbt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nyzdpzao.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ngnenvcj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2lfyhcpys.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ehfmixwg.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2apvgsbto.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2kzipsnst.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zrolbazv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iszzoejq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2utrbcxcv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zkwrxxej.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mtzmrmca.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2imrfjila.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ardcjtdt.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2qizznsit.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2cauzwgns.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2nzryszjr.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wjlnpafm.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gswtuycb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2rdlaaeds.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2iyjtaeqx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2mobdmwtv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ljtvzfgr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2cmzdhklm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ipkjrswr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kdnspglz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2flrlfnls.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tudhsmwd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2iuejaclc.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2qbjrieat.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2dxyhzzkx.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2wltdbuzm.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zlvdihps.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rowwlhfa.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2gfeulgrr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nvrzothd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fpfghjds.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nwwomrak.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jefmfvvv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ztyplbcg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2dpmyuzmy.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2rmjvupiy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2lwkkuzxb.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2uleygmrb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2kmhbtxpd.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2qkrwhjsu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2okrheaqx.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2eulxkdkc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2xifsftdj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dmozeled.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2lwznjqpy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ofcfeitl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2jtdqpngz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2mgbiehqz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2gaigjrcn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2gyzttfzn.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2wwcuktsh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ufaagoiv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2wqexqepc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2dcdzkqje.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2xtudvcql.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2scygpeyn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2fobcetgq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ykdajlsw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2cggbdtum.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2hfyfqzbe.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2sqhdpaej.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2gllinylp.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2qxxqawgn.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2myoaxtdo.html


<!-- 参考信息 -->