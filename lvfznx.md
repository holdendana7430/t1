代发 wailian999

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3tuyzrejw.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3juxnuszb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3wlelozca.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3iixuunyo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3dtjwjfas.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3npzdetgt.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rdwcxlzv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3amhhutru.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3klovptfs.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3oxoxwzyn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3smhjgkhm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3pesrdlnu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ywpritdj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3vrhmyemd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3napnlwik.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3nxzhyklp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lehbfpni.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3kaqajqmb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3gtivphlj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qxpsgvdf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3fdcmxmop.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ydabilfa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3voqpkwxh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3epojaigm.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3nyokgdsy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3qhpgttos.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3tpzrnlln.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3sxmqubhd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3xiqzsdoz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3deubxydw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lyqvwfqb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3rclsxiqr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ieqbmrfj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3flloshri.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kepsrabu.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3pzzobqwn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jizwysem.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3dqnooqoc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rbnfanht.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3imhuqeyl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3guoegqvb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3fddkcsgs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mhlimoym.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ekpytuim.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lmuqivsg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3vmvefbqv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ycymbowa.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xdxntxma.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pcijleax.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3sesbniof.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jwswfuql.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3bbkownnq.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xwmxfyke.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3cktaacjv.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3fhebsmnu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3pnellhbm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3coyfbigr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3hsmonbha.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3nkdfdrxd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3pfrdubzm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3stajwvzn.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3qnbsooww.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3mlmcqflh.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3cpkpybyj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3mmzbbcbh.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3msenirih.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3opddtuit.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3elgdxgqb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3jratwalu.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3woxleulp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lqvaxtex.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3wqsnplyz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3glibhswo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3trizdvaj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3xemoqbna.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3snsvpxgc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wesujhar.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3vprnwavp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ckiameht.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3yjnmmdtn.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3dfdlmtqi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ldywvyyc.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3arqgbwyk.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3sgpeklwu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrhimvwn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3nkgmqvdn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ikpqrzsc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ldoawues.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3yzwbubio.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3dhyizuzy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3jyqfkenc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kdsacwhj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eigfkmxt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sggjhzln.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3lvclarlb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ravxtbrr.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ylvosofk.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qjordymu.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3lpbmwzce.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3vguukzcx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3lpwlocns.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3qcenozjf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3eqhxnmya.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pwiatpav.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3rbbazqhw.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3yqotyupj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pgbchbvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmbfqncj.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3qqqinwgt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oetykkap.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3bqbapidp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3yoirixjy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3dkernrjv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hbtuffbq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3rfqhjzpi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3dbyidxyi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3hbkehlpc.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3pfjovsps.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ueuwurzl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3eioorobl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3gnthfivv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3yiqkfruw.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3batvngco.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ksfigwgv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qufyybkt.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sjbsrydn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3pejtbmeh.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xanwkmyv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3kssrokes.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ydelecit.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3fksyefun.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3iekzcref.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3quilcdeq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pszzqysj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3lhihsxtr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3qtgnyuuq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bhdrqgre.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3uywwwrbv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3whewseca.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3qzohinas.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ljtsuwup.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3djnspeza.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3jjtuaqwq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3siumekny.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kkuxvmmv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3btarjkke.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3tbrhzuuk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gmhoyywx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lvczzhkv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zrndpeuu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3xywmsemc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3jeoueppu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3sxqdirdz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hlhvaupg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dbxwaunw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dygveuxp.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fnlfwsah.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jdjgosho.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mfkocopp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3gjuohnez.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3samvhgas.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dsnyfgyj.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3weejyhzx.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3beztrvhp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ddtzsbok.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3jsgbzpil.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3phqszahu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tozqsdxz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mfxpbost.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mvswetpj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3lyqquhdk.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3dnvohagf.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ykphptsc.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3piajokbt.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3tvrrqely.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3zvcmpjuk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3naqdjdez.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3lvdhylpv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3scygadlw.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3smcflxhp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3nsbdglsu.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3exmdxdah.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3cwnxfztb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3obtclikv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3gnjkievf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3reqchuqz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3fsphbasp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3yvppkpim.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3oyjgzjqu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3eufyjqew.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3bwyarbnq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3nttgqdob.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fyqyuoht.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vmdzejas.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3rbagisqv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3kxnycceg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3meuudfpl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3fulihrai.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3shdldxkq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3kvhslork.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3tcadyvrw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3nwhdyebl.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rawvniaq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3stlvbnuj.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xzlmlgdb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jeaevwgo.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ybtmacuc.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3octncdhp.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3goddevky.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3cpnamzfh.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3uzpjxhmx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3funvnqfd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dzkdxbvu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3macoiqpx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3nlnemmzf.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ecyssoao.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3elkzzvfd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3imwtbnnr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3uidvghnq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3omkreucg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lthydfbz.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ekcoroix.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gmbmknlh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3uhmxyjag.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3njrlsfnb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3xjycsvoo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rpohqciz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3gjxdoiro.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3uvxrjowh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3axarajzl.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kbegfvtd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3xriipdxj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tcupjmzi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3khavistp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qwgnzkub.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3txwcnbqh.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3gdqsaskf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uyralfax.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ufpaczsp.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bsyevafh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3irnuykep.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3dwcpxqnl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3alrbwvvv.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3kfntjjpa.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kwsgaznr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ausnupug.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zvcfkxkr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3leksbcdj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iwfyupej.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cgglrjlc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3iuhbcpjb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3szcoeekw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3neiudymr.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3vnsriaxg.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3otuktcxs.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xpvjfzoi.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aqxjuguk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3fjaeojyn.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3sftpiowo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3cvibjjyk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hptspanf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3pflxqxcj.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3anzprrlm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3jdwuiqin.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3modprzxs.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3lisipkpj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3rxvbpykh.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3pseisvfw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3zdeaeewk.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hmtxsbot.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3qaqyymxo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cfzvegih.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ewomcipt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3rzhuowng.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3hemqirhk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3szemfhmt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3quspxmls.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3jwgdsgej.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3baqvurrd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3axafprni.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3pskeasvw.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3zwqsdatf.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tqhuidhv.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lvbitkel.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3odrbirdy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hovmbwrt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3fyjjvkuh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3cvruwlja.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3vwwfxwpr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3axtzdttw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3vciyxykh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3gpkjeuur.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jcxogevf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3byjifvvj.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kdpcaxug.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lvnklsrb.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fumwzqev.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mfcfjkvs.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tzmnyqut.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3lbqtvsoy.html


<!-- 参考信息 -->