代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2kcfqfhon.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2wzxorify.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2madpeqtn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2kbyzgega.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wloimezq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2flleofvz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oogdrqmh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2bafbhvor.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2rqpryaws.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ttjundnw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2cfjdabrf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2rtawimqn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jalnhaye.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2egozlsut.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2wpkgcfpn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2hosyyssm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ujrhdfgm.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zvgwspcc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fvacrqir.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2dmxmsrrh.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2obagdddj.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2hdytybtk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2khmhpsib.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2cnteafgn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2zvmvoaxe.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jedjhesm.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tvgpbtag.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2zozwjlhi.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ryahqolk.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2gvpnxbdh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2zjgbrahc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2odcccrmq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wqovfuoi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2eabuxymp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2wjwgqebd.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2hkeohpjb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vrzxaydz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2jigqckds.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ejvkicum.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qqaqunxr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2fmabdjun.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2nucdtwqg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2zvlszyjt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ickuvspm.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2qevzisun.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2uvdjxzqk.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2etfggshn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2oirauqtq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfzzfxmt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qaukhqnb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2axmabugj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2enxywywe.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2llotklog.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2bpduisug.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ioewxlxw.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2xmkweekj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2cfvbyhal.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zmzjamxl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2tqcauafk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2hsvjrgbw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2btlzdrln.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2cuhegguh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kpnznoej.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dqmfahbs.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wdrygxpe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2gzyxnfwh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2xtobzlnb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ksabsqpp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2uggonfhc.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dbxplkwr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oyjhesnk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2kljograh.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ymeqsmca.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2tmaslqnp.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2jhtgbyqq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2hpomjfnb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vwrmnaxu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2pnogoyil.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2dzhcnkai.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ssolfsmm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2wwxxdurh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2efgygqcg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2wtvlpsgj.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2txavyyhb.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2blhvxhwn.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2kmaofweh.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2kxmgganu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2jgnmtwab.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ytajfwlt.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2eqoirbhc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2osdyrwdb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2hxxckvll.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2tdliianj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rqbynljt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2wnczkazi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlfjepon.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdsypccd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ywttmlit.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2oszmiizr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2spzxmobd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2oatmwfds.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2reodspyp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2osobczoh.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jzymfalh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgafhumz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2dtmrfwiq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2jebqehkj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zbpxmdzq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2seyazkpv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ilzzcddm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2tqutatmq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2lsatyxpd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2jhzshbdz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iinxgzpx.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xxhdulhk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2rkcpdzon.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2nfceicxq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2wybfgong.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2xurauazw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2rasvnwyl.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2qchcczqx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2mpptfcqf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2uqjhnlad.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xtmdnfme.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ufcfxcth.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2nwfgyrzf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ftxywvej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibjmrjwn.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2qypeaxya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jfvnuovy.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2usgwwbzj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2bzteglmf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wsuinycm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ghisghky.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2wxjmkmba.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2gqkblyde.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2cfsyqxel.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2nzruozmx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2jhrxjkvc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2kitnacqt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2fztglpql.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2rdjvyihk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2jcuymzci.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xxzxenmj.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jkpdhxrs.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2fhdchcjp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2nbusorgf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2loqczswr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2uhwavmdd.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2xdjjijbj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2cfqvihta.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2cbqucpgf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dwkcehdr.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pfuztpqj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2wxunszvy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2gxgqmgwx.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cyxnyual.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2icwecbgz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2zvwforig.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rzmmoutt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2yogjrxid.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wuxftefe.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2odhxlhwf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2tjseusxf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bqjanopc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ywimpgcs.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2nufafhfb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mrhevlgz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fgfcdnqp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ekcdgior.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2iujdvven.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ssywyclj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ythztwwm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2owlsikxb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rooeixrr.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2udoycovn.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wsouywdr.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jnhtjnit.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tlbdnpvs.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2gskfjgtb.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2orkwpdyh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rsyheqya.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2svqoqbpu.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2nwskargr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2hwkohtco.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2sepfdvil.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hojotkgb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kibhiccb.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gxmzuovy.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ohdrpbpj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2mfenhkbl.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zkjoelkj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2taqhgdbm.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2hpuavely.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2aizedrva.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2uezylaki.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2hqoablvc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2nndjkdwc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2rrjidklh.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2nmvvpvlh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lvjmtqpz.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2juqqwpse.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ypgmziyn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2imbeibhb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2molrnscg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2eduwginw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2mfqhmdit.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2jegifsjn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2klcheylf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gpplxphb.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2bojrljww.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2wgvyhgxj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2pesmwwov.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ksbpkaap.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hocwnkye.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2llmjzgzw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qpogrvrs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2hkxpvwhv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2tbyarrwh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2xfsdstwf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ckszapxw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2wazwynbm.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2kzmrwegd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ngfqymve.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2sqpzdpwn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2dmofyoti.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2uhubeusf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2zvylxeik.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2pkmourxx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2awmebarw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2cumloedb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2facszcfw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rqmdnyfu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nbqyemhr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2yooowfup.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yuulzccm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nptuvaqf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2krigstju.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2xaselmss.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2dzohnvum.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2wmpyzuid.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zhljdqvt.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ankmydxa.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2amkylszf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ukwjqlbz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2gckpccgg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vwvmwhpc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2trzbzchr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2moqneyqd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2saigrvrw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fhlddvzf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bcpyggnj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2wygmrtaf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ljhpfvtq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ibdtljhx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bljmifbc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2lclchxcz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2lmorgphu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hpwpnndu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jafntxgz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2evwerize.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2iyyejlkk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2yfqanmpp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ykvuurfw.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lvvenhag.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2almsdinm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tudondvb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2erzyctam.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2phwvjlac.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yjqudcfc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2mfbpnmce.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2cphdkvga.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nokdtrvb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2xiirzhir.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2taglrywx.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qwvarjyo.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2wrwdxytr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2mrtemrfi.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2wghdwgyh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2czckbpdc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tdeijnqe.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ehzpatpd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2hifanukg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2zyspniin.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2tgmvryzm.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2rtvkmhur.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2gxuiopgs.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2haseymic.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zozzfjxr.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2wmcppetu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2gxkxhwng.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tvtbazbe.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2liutmlly.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2pxtptxki.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2vtnbripq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2tfgvywgb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2pcdpudca.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2pwmtrhai.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2isxwghzc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ioyhgive.html


<!-- 参考信息 -->