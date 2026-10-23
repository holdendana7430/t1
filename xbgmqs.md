代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jdedutgr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxavzkyo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qfrmuumt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3sgqbayvb.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3jdhqywpy.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3amiknzui.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gdswwdpe.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3nqttfqnn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3lzxkeapu.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3lxicghkn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3yfnjinvj.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3dmqwtlzs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3fzxmgrmx.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jspxwxxx.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3xhchtfeb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3yrbgemia.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3duxiiejs.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3uimdoiqs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3xlcjqlie.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ojcawlup.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mdnzhsao.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yqdungrq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3gawzgsqu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3damtmbit.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3gwrmbqbv.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3bnmsuybe.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3vlhdlgqg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sfeumzxe.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3bsbntbkn.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ankitljm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sifetdnk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3zmfzsiyq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3mgqpntau.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3zelceobn.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3wkeyqtdv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ooqktkmg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhgqaqen.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3fitoupty.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gurttlqg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3xwwpbhor.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3svinkjux.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ggxzmcsg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3seleqgte.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3hvgauwzu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3hbkbwqzb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3hnsgjbtj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ozzcnnbs.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3sjpophan.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3xjsxnwju.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3qqibxkrb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3gdrxxdrq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3duuxbcks.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3dxnwfnuu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3raoicixq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3yrrkiksv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3kninbzwa.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3rorfbbeo.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qvypogsn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3erezwalr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3vetgysar.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jjihfzpl.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3lumfqznr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3adixmtkl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3mutromtr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3bbpvcyhq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3wkelmmti.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3pgptmqnd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3cmfvdetz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3dxwmkhzd.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3selqxpdz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3uaxkafjj.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ktrmcfou.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3zrqustkc.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3sseilnzm.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3qbqzxbqi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3vdzljppr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3lzqwhtri.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3awuguxpq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3zlhxbaex.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3andoqevn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ohaiclin.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbnmxome.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3duziryks.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3opoqkrxi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ethiqbaa.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3nkhlbusv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3jdeuobkh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3talazsxo.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3jbjkpacw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3tidafccw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fonsevlz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3yhpamrxr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsgvatef.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3txftdrlr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3aurtngjd.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3orwdeicv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3uumlosqf.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ndujrgmv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3egzgjgnl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3amxqupdu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yuyslajl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3entiqcei.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3lqpdzmrq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3oukaxlcu.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3lslfhxbx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3otqyddqg.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ikkgutfn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3rjjlocpg.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3dufidpix.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3bigiaigh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3cbzjtxzf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ybeijcsh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ikgattih.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3mlwnwava.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwsskivm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dzzigygw.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3bmzvioei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jyipigey.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3slfqhidr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3beiiydfq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ptgnkudg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3chyavhwd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3odxhxqxz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3yryyyfta.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3iohevbbx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3htvrxazm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3nnvjshik.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3gfwhxkyr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3jbjybzqn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3uxatfmuv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ebpnkedn.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3buhbwfdx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3urycoowj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3sjuffixr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3vaepxcdj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3tqztjgst.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3jtzralfc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bbmuguly.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3wpowynez.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ruffshmh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mkcogmvw.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zfhufeyg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3yivzelbb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3yeaozdpn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ptbeizct.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hflybzgo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pxgpyvuc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3rbkiijwo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3hctblqap.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cfjfgocc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bxuhlkpc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3vdlaqwsp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uyiqdtdh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3jlbpqqym.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3mfsqujgv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wpjwpyot.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gmnhpnxd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vrlxqyae.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3vhofzdbo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3rirughnc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vzsdqnvs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lyzcfdtv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ynovgtmo.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3florlzyd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zfviuyuw.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3vcbjojvs.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ppuhyguk.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3lcfzqytj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3zidlxigw.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3uvozpvvi.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3bybuldzm.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3rqdanhsx.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ltxazvqd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3emospgwq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xvtvskxg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3priustym.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ekfraksb.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fwwfnnoy.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3fnnkmqlx.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3znglpzox.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3aaqfvubz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3lwehciov.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3myzuxsxs.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3jnnhlrcs.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3apfkoluk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3mifjnsts.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3vdhzugtv.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3avvtxnfi.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ifmlhyrw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3efrzgjzt.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3goowywpz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wtwdiivc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3bqgkczmu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3oyuqzllr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3axlmnxms.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3fwatbbla.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jvcullqw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bhcyldfq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3bvrcsghs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3nxzyqgvf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wxnncljc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ngdxbhhq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xadotdsz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qyrhvmsf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3lqunijvy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3bmncirhy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3cdrorfjs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3iulactnk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3gzddkbuf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3caxejmjy.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3hulforbn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3cfmccxjp.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hogcblpr.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ptgzkzxu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3lfczeceg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rsrissxv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3lcwublmf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3aqlwgoog.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3anuxhmef.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3zrvncajo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zdayfslq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fdlxyplc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3hslxoimu.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ugoatpnb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ywkbpjgo.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3oshnudcp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3chkkekap.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nxpfxvjr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3okhnmuwc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ynelmgkm.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3osuqebeq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lwqrndbw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3mjeheniy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3zmcdajxz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hzcathlp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3jlwglgzf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3oaxhphia.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gdphmmzb.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iescjokw.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3baiqpnun.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zavwykgi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3zlukrzsy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kjxiovmk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bjzflxzd.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3jmsqilvm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sdmuuxea.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3insytabv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mdjbsfey.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3blgqlqje.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3yihntlrm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3bbosofrw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ojxjvcnr.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ecyeosfx.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3pnhzsvbw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ahhzlopt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3vmjvellf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3taufszth.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3zpfidcjs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ukjjbqqi.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3pvuedqvo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3rwakolqo.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3cdqeufke.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3nhbxymel.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bieqvusk.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bnhzxjho.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3uyiaeysh.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3aujxzifc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3goekbpwe.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3exmgvrqk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3vmivaxxg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3mxdittda.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3qvtqpqwx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3zzapvcou.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3kdjrchuz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3rchjtcjv.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3hpkgxaze.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yrvxmczp.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3jwgjgkuz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3bzsysbch.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yfurhalt.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3sbdatmdj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kfyqqkvd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3pixdcedq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3gjfbxqus.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vftspwbk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3odjwmpzm.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3qplvhfrc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3wnvtycou.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3vzbhfbnh.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dvglrdjy.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ughvutro.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nkajfnrg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rlkyqdrl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xphgxpwh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3pbxrwcli.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3sxftmfqc.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3xkoxcxhi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3mbjoxfvb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ufsyliad.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jpccqhyy.html


<!-- 参考信息 -->