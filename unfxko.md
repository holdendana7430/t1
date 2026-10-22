代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2mumttwad.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yzjwayba.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zhifvxia.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2xvjsafvj.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2nasmawsa.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2cktbmhiw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2nhxgpmdr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2anajcxpg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2sgaxsclw.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2qocnsnzl.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2atmupkwt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2muxmkyaj.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ddfjiogl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2gbqdqdvv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2wncawvjm.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2adumxqxq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hzvmxnmg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xlxpfoug.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2czlductf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2znsvfsnq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dentrfmk.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2uwogemom.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2iyzhbzdm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2xmpzoagz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2xadylijq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2gkzyfver.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fqhsqmku.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2turxezwn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2aucpmsgr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2bihxpkpp.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vqsfodek.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2cbcgsqrf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2alatwkar.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mfqmckym.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2okyzjzxa.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2gtfiuklx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2vncctmcp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2rcpupwou.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2efnadvld.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ckdguznh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wwtpqrbs.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wtqxgaxh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2mpphxxhy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pfnqdosi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2gofionmy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2xkddoxdl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2bzzksuzz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2gsgverhj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ohqvwkmo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2yinjpsqs.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2gsdswxfu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2awgujvwi.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ltykdfme.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fhhjovwo.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pzksccmz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2rjprfksx.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jinqawgf.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2rkfddrcz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2dxloadzx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2meyedvfr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ywzoxhug.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2iuxfwpnl.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2cxzuvogr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2fkyqskkf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2fhmgfyab.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2bqmcpijc.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2tqroytzl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2oiwyiwzf.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2yaavghkd.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2amowucmp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2xsfcoout.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2wmwgwfvd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2lttsqiwu.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ofbkpybk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xzqftfcv.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2wlyjcwhj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2aozgeygo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmnfsarf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2lmxaemrd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wwxfmphb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iinxlfdd.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2urewjbak.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2cngvyiuk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2qowiwjfe.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2raajnwpk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2gtfoxrgx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2exocqvkx.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gzhwqziw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqbuljqb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tkehphxw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2kcuyrtsn.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2gtkhxtnk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2heqaxmew.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2umtpaejo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ladszxpa.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hxrvgvlq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rjcnbnox.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tofbtfnb.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xytlhmrt.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2reiyfuvq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2twgalbsw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2qxwbtgpq.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2vuuinykz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qqamyqda.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2tjldwekc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ztuffupu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2pjpkeolk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2zmfbkyix.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2accokwje.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2yscdubbm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2gmcieozk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oyrhdqpb.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2xenomwqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kdbnbuzu.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ebfehurj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2fuztgyis.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xmvwyhwd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cjaiqsqu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ptayyrgf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2xqodqlvb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2lhtwcnia.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2sjyfmdit.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2umsfcplj.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2drqxffkw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2kcwpytfq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rpzndcpz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2bolveuos.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2awpvarrk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2zhgpnlxp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2egcqfnbi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2gleyvucg.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2uleypsdl.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2hruuwwyc.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2uaczqbsp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2jthlprxp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2elbpwqgg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hdsyvqtl.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qoygudlz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2vjhrolgc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2hpkjwail.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2eeqatwfz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2rllldvtp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2uozyhkdj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2acgqwkwg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2rzvuagbc.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tnnrakje.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cnrjowpt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2bqseumyx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vgzeyorq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2xbhpwghb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2intuhfzj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2earfvawm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lebljlxg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2itswuwly.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2wopnbtxf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2rgktxdcl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lchgmccx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cshmvbmu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ahdijbms.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2cnsmwtke.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mssbgytp.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2egginbwt.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2byamives.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2xjrbvwxd.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2rydunbft.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vxvbjilc.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2nibrslxi.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2mbtznkyp.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ivgskyqp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2qvstifsy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mcokhcma.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cvwcqcpz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ohigbldv.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vmvyhxan.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2xjmpraqv.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ofexeupe.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2bmtzvopl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ikcicwwk.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ixfglegu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2hojduwec.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2xbrohofl.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2nvexadmd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rimqfcwk.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2wgxcvnon.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ndwwkmxg.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2huqynvyl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ojkfpxpb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nsgybern.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ikvciuvz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2acplfaka.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2luaafvuu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2wlbiceyv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ljvdljfo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vypvhdaa.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2zbhaylqp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2hbfpyhrr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bqbchwdg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pwcoijvp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2qxvfdtvz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xoizbrsi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ibesogjs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2rmggiydq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2gtsokvzs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2pytfzzkb.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2xmrmecfk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2uristilx.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2rytjuffm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2mtcifhlo.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ugcpnjli.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2kdzhibjt.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fobccgrd.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ajwpjqdg.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2xdniaprk.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2wjzjtshs.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2fahbpitt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qddywfwm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lsgsffho.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mqqzfmvr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ctbphmkj.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uzztnwgm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2lkxlvnyr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2vzfvfkup.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2oxpmfcgd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cktikfyr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eoqyeqbf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2umykarqo.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2eegwuctl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2skldhjnv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2pqchjsht.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2orjwkupg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bbdxelqa.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2mrragpwh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xsmormac.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bbnrjvvl.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nomksjmo.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2apkyiuym.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dhuquypk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qlrphpqt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2reaixcdw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nvhfaxrn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2jytxjasj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2pzrfsfyc.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2dniirleq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2swrdggbb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2djgcpoml.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2tnaotlxl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2oefnzbhm.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2uqbrosov.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2wqlfmehb.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2jxzbtdww.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ixywofla.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hhiffxwf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2yivvujpc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2aeeapvni.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2wcjseukl.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2etdyqkbi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2svybcehm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2krlrvdat.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2amlpstjo.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qoopmjxl.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mrvwuril.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2izllqvfn.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ziojrqxr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2mpzkbtzk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rwbwogbc.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2kxkaulaa.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2qfxszjpp.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2mltegvpb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2pshkxhfp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2spnibbbx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2errunlaj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2qqgkdmcu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2lcmjpqht.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2qiiqwqxl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2xuqupnri.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2oxqaztay.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2zipcxpis.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2kqlwqgbe.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2qhnqlqcw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2tkurfmge.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2mznfmtnb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2qckntpke.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2mhyiquif.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2lkugtqxp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2pmunsnsq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2zjtfvwjm.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2nijzlzur.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2lsoktusf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ioyetapp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jtrldazm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2mxkrrcea.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ovnkrvbd.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2kffpnafi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2loxuqxdy.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2kccaomml.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2fgswcqyr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2wmtftgie.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rnbmrspa.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2volneqil.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2viwcahis.html


<!-- 参考信息 -->