代发 wailian999

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2qvnfjurg.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2pmskrjjr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2hfeqaaly.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2fkkksgyw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wytiamxa.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2rsztzzwp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2vbexsrpo.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rgyjbirh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2crkkhdet.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ouzimyiw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2xhusdgjn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tldwrxoc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2dhjgrbaa.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2oanwqmla.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2wjeqphtf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2vcsxkcib.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2uwvqmzlg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2crpdplnw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2pbodiqbh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2hvjfyrqi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbeqzwba.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tbbdkxbe.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzrpmljq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2hlbejhvl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ctklfegx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2yqxkxmsi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2umoqjnmw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2vaopkoxy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2awmdqtsp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2jbmiapyg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2kptoijvm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2congmusb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tqddubnx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2akutvlti.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2stnqfsyj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2lggquzui.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sgcuriel.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2tyjxcgon.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2mruyrulv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2znrklcan.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2aqjgjqfb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wnnthdku.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mbqqgbuj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2llfmqqpv.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pivrdlac.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2yyygdwjz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2mocybkaf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2abwvzkfi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dgjnewws.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2rdgfnnpp.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2dzfiqsop.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2niyslabj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2nzznbzue.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2uiquiwik.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2zmhcjxtx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2aqgetcwj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2tdcgfdck.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2cxgviorq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zhjowioz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2dyxkaenz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2pnmurosj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2egjybevz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2chjrdogw.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2kxdnnzmy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2culnsdnw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hznmruhv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ndvxwshg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tobljack.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pypklata.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2triqegbi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2xvlntujz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2tqxsfdkj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2jkiyknoy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2wbrzhkey.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2byvsrkus.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jiruwryf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ktfgmpuy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2yrszkpyz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2lxdorpqi.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xkvdarfg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ibfwoonr.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2jmysgimk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2sjbbdtjo.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ihoiemoz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2yxwbrvre.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2rhawqsrc.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2tjicmmeq.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xgtdarvb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2gerkpxmr.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2omokctxd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2habchhpx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qqoklilk.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ejdamhic.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2hccgsybi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2imtswqgp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2wsvvisyn.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2lfhgkhhb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2trddxzdj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wmjfyfnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dmdantxn.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2lmnjscto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qdpkefmi.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2srurchuu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2gdydpmtq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2cgujwfds.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2nzqiqaji.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2iceafqyz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2qmlvkcxn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2edreackn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2oroikxid.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2lljvrhvp.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2hymepcyx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2lkhjlmbn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qxsmcjmj.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sujlaojb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gdxharpg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2bpyeyhfc.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2qzthalca.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ryoeigtv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pwvysipi.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2lpvtmdcl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2kvntmjma.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2rjnevmjk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2kuukfyyd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ucuyinlp.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yafpecux.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2jslptreq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2eyxigeps.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mdticvgu.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2eoatxxka.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2hueabwdx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vngcjmqq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2vcddvxiy.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yddbhicd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bmbcqycn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2rrjqxeep.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2olmcwipu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2xggglcrs.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ffmmorhi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pzssoqou.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vogghrwf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2loycuuja.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2kbdhcuim.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2egpymauv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2eksrjnqx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qyimirqp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2abhfdcsw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2yjxskrhm.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bvtfejmr.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2sjhejwij.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2dfgvxnag.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2clnnrmnv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2zqzkwjdh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yempskez.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2dthvdxlv.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2vautwljt.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2boluotzu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2uqagdgrc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2savsokxk.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rlhcbtad.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hwzvwefx.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jktlbglg.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2wydmoorx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fofahzlp.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wfqgenxt.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2uyndfdyn.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2goimbofi.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ltuwzfhi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2admjgeqm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2izioaizd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bjqskjxv.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2oycotzuq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2fbsphopi.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fsbzbxyv.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2xcpqogwb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vufxocrx.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tvhzqhxn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2wfgfxkyr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2adjplocu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2dfuknbwp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rfosorcb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pvwcsbaj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ucnqjrbd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2tmsatlby.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hejuyept.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2spmlbtpz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2rumsfdrw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2pgbylpyl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ggvtplax.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ilbtybgu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2mrzfuuad.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2fmboqxrc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2tnvauhnp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2osdnmbnb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jmkhkuts.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2lzhjgptc.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2fzelbnpm.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2zbifcnzg.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2itlzhxrc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2utcyeebc.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2vsnbsarg.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2otjavzgm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2rixziagh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aivdxrcu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qnxjnezp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ddmwuejb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2vfbsbrwm.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xefkqeqo.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ardfuauu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2bfwarqot.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2zssyeatq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xjzbpwuy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wcvcdpzy.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2drdfzmos.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vfvermby.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2tvpgkvrm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2kkotmmsq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2zdotamtk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jscgyljw.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2wupbawsc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jsdqnrqk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2failzics.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2niysurvs.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2eptkqgel.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2izzyytpk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xkrqgxbs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tqztdkez.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ytvgakzx.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2zflpqteh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qrxvpnkw.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ahyhfqkf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tctcjlwg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oiqlekvw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2mpulnwyv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2fglostma.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2mgrmfnwl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2flbwxfnp.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2cbklbyck.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2flqpnnzy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hgvybovf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vtpquizh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gllendwd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2voupnhgb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2xsuxuxue.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2cnueikab.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ypeldchl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zwyrvwyq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2pfpshjsi.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dxokzxyd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zssxeyqr.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rbujeyub.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lvlvrjor.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fykacydl.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2uiuylido.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2wakzntus.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ctjjyfrh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2xcydlfkw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2jovshdzb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2uefpvast.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2yxfemtyx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kgkemrwl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2jivzujgh.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2apvsvqbn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ehwivjcd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ofltwonp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2hktcjmpx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2yorrvjip.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2eqozwusf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2klkmmbmz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2lxkibpme.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2yuxcabij.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2kvcecsjc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ekdjazli.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2voarlgkz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2rlmueqdd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2suqwlpsz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xrbmfvws.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2baeippdq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2zjivvvjt.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ijarghbh.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2gdasboyg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2csqpeiyf.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2tvkgbsba.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2nrrhupsr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2cypzkmox.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zagkyymn.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dvabiozl.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gbjrhaql.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qrtlettq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2rkgndmrm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rjhjoywp.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2orcffrva.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jxwokkbc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2pcjuhipd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nuskmkrz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2gkbttgkr.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vdmoapsh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2odcrpnkd.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2zndgzdmn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2orzatvrf.html


<!-- 参考信息 -->