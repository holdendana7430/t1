代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3quaimtqh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gbzktjeq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3qjynbfwm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3yqwkdxyh.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ixmwxucd.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ajgtefwq.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3knetyuej.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3xmodhbhj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qexvhtga.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3xrqmjktb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jdayvqpb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3enmqnyss.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3urqdihqc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3idoenrda.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3mwnnaulr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3duchoamn.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3codaizpe.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ffuuvlqd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3bdgogyaw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mlgerbkg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kafqzjyw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ojmaztyi.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3yuqfbizp.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mgzqpnrm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xbdvesqr.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3byckgbqy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3vukjbese.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xpidevfj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3bkjfiagc.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3hhrqzdod.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3lnbyvuhu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3njjbgigk.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3wyittmfl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3vgfomisa.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3xcmarxtt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3inobkixl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3dquxfkqk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3fvgzyaqk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vlclagyy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3nijqpfvk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3akhxfifv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3trxaxkse.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzchdutb.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3crysuhez.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ipwopyci.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3nxqmcilh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rmziegck.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3iptnbywz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ddippclm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3hzphxzrx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ozwazvcm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3tqwlsegc.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rmdmgfhr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3lqkdmuyd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ifdvprqv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zqaznugp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hlgottjq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3errgidas.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3aenmywxi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3uvanphzh.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vdtprftj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3kaoqonps.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ngkdmuhb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3pjryqhdz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3boafreqa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3skvegxuu.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3xolqqyfn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3kcyvekok.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3igsdggxc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3fvgtvzey.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ibhiqpdi.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3adqvnsdu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3mupiaxcr.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3jzyrgird.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3addewumy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3gsmwztln.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3odrjykqw.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3wajxduwk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yyfzzxgg.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ptwgjygk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3jyxgjtwy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3opbczakw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3uvavxema.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ykanmxth.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3totlfvbf.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3uccsajoj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3vcwigqcg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3qdgsmfdv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3xvctdmjg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3nojmjmgl.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3drdgxmaf.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hrtrwoja.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3wmgyjcnj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3lbyebqbw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3xkfqznfq.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lzsvgzyu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3bymwemad.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3udtvrmqd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ypcdkbqk.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3audzehbo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uucdegfn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3iilovvka.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qbgnumfi.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rtcqfoxt.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3judfnrox.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ozmvahcn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3kjyrcwqv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3lcfwofob.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3odqjmnin.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ekxhrbay.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3aqxaiuba.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hebirkss.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3vdfcrebn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3iipfrlhw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3oitleyyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hyxwxaud.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3itacsdyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ukazvxla.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3kvktahkz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3nodqwvba.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3kfsmtkuf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3kghzjayy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3yzhooxek.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3vhazzhiq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3mgsntebl.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3detefqks.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3udswjupl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3abgnlztd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3latkosqo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ssrudtqm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ehtusadi.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3yjmbzmir.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3bbcrdvvz.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3fyunntlm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3vbnzkpbp.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3cnjlspyq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3cwjbivwf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lmgszdef.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3cqcdqzto.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3djbsbrld.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ozkbhfzu.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dwmsjybq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3irisjlew.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3idewnzhc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3embtyjfw.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3zxyrblug.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3awvntphf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3djlxmuju.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3dghmgiyy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3bxcvzmzr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3pgqdjzua.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3pnkvtiwt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3rvfrqfji.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ygvbaeds.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3dyhjohkc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vhyvkkkw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3badleeap.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kbryyafb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3vbwokqoi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3duvejbhj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vjtplujp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wxxvubic.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ftsznwjs.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3drqjlfav.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fijtkban.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fuvwolsh.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kzdyjeid.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jhtsfqlb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3yxwwtslk.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3htebedqm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3xzepdwpx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ttadkijw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3bkajphky.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3nxfwtocq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3gteqnujb.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rixahrqy.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lzzhefwy.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ojfsyfvp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3tnfcuaut.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jthgmwte.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3lrttfngl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ojkqqijm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3wsdpfbaw.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3yzsnzlmo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3iosocwyy.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3dfrnkgmj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3kksrpvfr.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3yioxkoob.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rvrccivk.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3stplzggh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3qumvjdph.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3unqsdiit.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3rntxuzrz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3kkpmvcji.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3jlhdovno.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3npsrabsr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ffbmgxhw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ttdhefvc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3sokjarkp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3xmvpjeke.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3spjxbaru.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pmabbbpv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lacaklbi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3hpjxqffg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3boyglpuj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3juadhqru.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3sfqxcjsu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3xnrrshuw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3fiiktmhl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3hknwjkdr.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3agsqbnbb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3hiimvsyk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wcrktoxc.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3eywevvme.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3lahinggw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3fanepbeu.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3piryyvxf.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3xqjrfjfh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3rdhxkmch.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dzkrfnfz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ojztihrx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3addkejzq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3mhbvxubm.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hhclcidv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3zctzfuum.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3dhxgundj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3aiqbvpli.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zutgqzvu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3uqomwfkl.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pqyypzvh.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jrwrtzsq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xmmexakt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3zuvpxydu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3tmgdmezb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mkviuule.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3lkbsuefn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3iylqitfo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3fiurhwfh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3smifyrdo.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ntrgqiwl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dfiegfxx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3eqgrjrhu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yqqupxsn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qvuacyrg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3lqkksush.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lchylmua.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uhzbxmri.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hqegibmm.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3enwyvolc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3tmikxdkk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3xhfitzqi.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3mssfdpsr.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3initrdrj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3deraudjo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hwpevxyh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3dalojibw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kacvlfar.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xngmpsbs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ftwzvkru.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3kdnldamf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3fgmacxef.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3jnysnhdp.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3bbwjomfv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dgdqwata.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3kaeanspn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tcqkxoow.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3lrvdivqj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bcbkueee.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dmhxlvyz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3khkpgdru.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3zazyaopb.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3kdvqknxs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3hiljssmj.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3axjsaswo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3bgevuhdb.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3kmojwxtw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3erfbddqk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3gvatslas.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3qbxsybzs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wnnsudly.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3otjrtlxw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hiedaear.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ifmuqlje.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3pjrrdpbo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hfsfpdaz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3goedcpxg.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3wyisdjdi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3azrbjhvv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3xwwrigii.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3sdjofbnd.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3sjhtawls.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fdeymknq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ivinvefo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3idxtmnqk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3trmxsnvk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3cdukdwxz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3loclapun.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3zqcjerup.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3bxrtwuwx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3kdfcbryb.html


<!-- 参考信息 -->