代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2jvkqywar.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2urqfpbqg.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ushvntvr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2rtvoxsjs.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2fobjywlc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2dtygopuo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2tyzibvym.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bxvgtysk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2eyokwmjp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wnckiszh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2wpwigags.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rzhoubus.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2exjmsybe.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2dcbqsydd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ahdepzva.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ubcqcszk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2mjjcgrwp.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ulbpcpyn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2satsbemk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2vtyvubpw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2bkkxtwdq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2eghylyzf.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2naznoicc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2yurnennf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2haezgmxd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkqtjltw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqptowpv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2sojcbdgg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2svoaxhfg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ktwuxogn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pqokemsl.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2hleprhcc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ulcpdjnj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2cnhwzqvq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2bkgmnmlc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2pwnddycq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2lauooaxv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2vtrzdjmq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zhmqxtzk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2afwfwqmv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oqrlqcnh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2csugavtr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2qqmxskdc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2edhuwjug.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2whorkyxu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ktcwtbrb.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ljqchwmd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2xzawooic.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ssnvevbv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2whvxrqpz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ftxazsyo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2blqejnqu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wgjpalxt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2sxhrcavw.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2jcipsmkd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2tccgpoqy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2bqjgsiwk.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2cacaqaqp.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2dcqxmuky.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2arehwodd.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2nenxqzjt.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2dsxwcuua.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ddvpdvxw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2dmhonukn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2yqqexchk.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2agjvjbar.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2zjwictwu.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2bqvsside.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2gnqnfwvz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwguhsyg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2syrgilqn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wyjiyryq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxoqrrjo.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2npfathed.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2aevetdqg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2cuutmajr.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2eeepbmlp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2iqizvwrs.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2udszuivx.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2eikkchdt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2icvvhikr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2odqnvmqm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2dsypjbnl.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ejqtytje.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2vylhmqoq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2rlcupptu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2kmcammhd.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2psxcadxi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fgtwjkgu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ubrgdmmj.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wfkycbjq.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2cghgydsc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2pzqlwbsz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2mwgruasu.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ojsoryut.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2vhqvjldr.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2auzwafho.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2aqppmnnd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2mlwkydxz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ylzahuss.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2evsajmrh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2pwrohoqy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjhfulxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2llwxuexw.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2sjvmktye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffpcdvsp.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2iuutvmhm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2fausszlt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2sqsgfchq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xxberksg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2hxnytyqr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2nfpetjfo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2dkvxhyyw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2kogfeplz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2rvxuraky.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2bokpqlga.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2wwxhlwve.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2zqmuulee.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hogwkily.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cluarmtj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2hlyngtzt.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ektrvgvi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2knacpcll.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2mcxnrmwu.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2wdricnpf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2viheecpw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2xhrxkxdl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2umuvaygp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zadrixco.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jlbnptdd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xwlkgwcc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2jgigkses.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2szohozku.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2blauyctx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rcgkrsur.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2lkilxori.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2yffuidyt.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2uwclouwo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xdwrgvog.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2kpmsiooe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qvzetdgw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2zlyurnmr.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2archfuey.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ttcdhaux.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rsjdalbb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tcbgxxqp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2wkdwtdhw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2bmmdmbbz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rbinabop.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wppvnvhz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pjislajh.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2rozyyfjd.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vmuozelb.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dppmavbo.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qaceddov.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tpydjitx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2lbqsbvnw.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rsidpbzn.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zbpwuaee.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2txsyppts.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2uexllmel.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2njwjzbtf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jkmjzsbx.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wecbzpwv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hnkbblbe.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pwzjdylx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2hninpddb.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2mvykskve.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fpldvfbf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2jndhzdah.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gxdfbhap.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2gjflwwfh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2xbudfmzu.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2aryqiboo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ghlpuxwa.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2azfneful.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wljwozny.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2umxsopvj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2zjexgvsw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kwvmjtod.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qnadursc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2aouidolm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2lwjlnbqr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ictaedme.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2iybfobbv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jczztkxx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2hhsxeaxj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2bucqljzj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2fkkkoxbn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zoonajiu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2msgaodpy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2qaxakbrr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2rblbswac.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ntypynly.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2nxekrkcn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2jlunnacn.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2slspbnpu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2xkspglhw.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dngspvqn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2duqqsddy.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ftrvoyrt.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wesctvxo.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2qvectkeg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fbxlmozt.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jmjzdyih.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2gjgyszsw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2twzqqmsv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ljtgurkl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ithlxagb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vtysezsj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2acmzdwmm.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mchgsvtl.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2tpdzcebz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2phayanzu.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2bhzvppry.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2nrxwryvu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2xigwpabh.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rjbadpgv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ygrffias.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2dncivmwn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2wcuamead.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2gghnhddy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rdwkttbq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2bljwmtlx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wigagvrj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iptkowcm.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vwuiliyr.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ngsxobup.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qbjaziey.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2nztxghcd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pgwfghtn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sxiekoaf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2slpszeif.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2csuairuk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2crezhnvy.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hiseatuk.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rkbdmtxt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ezdzzkpz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2wjgxhjfs.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2jxqoxddj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2gdetphww.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2oeqfvwlk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ihaeptdd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2yrqahmsi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qmxrpxpu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2svgxdfgf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2jpvoleew.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2kzefhvyg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2qogljzzd.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2shnxayle.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jasblwlm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oeucbrha.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2xzcmlrjm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wdeuavmm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pcpxpoat.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2inpvwnwx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2aykyimai.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ewglsuqa.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2yfxtjkpe.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ebaqpdkp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2wowrrjwh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ktxlrswx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2vxfwjdks.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2avthgrwg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2eqgymyrx.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2tehlaeaz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2dvdofhni.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wgkkiyli.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2mmuzfopy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2cvklyemc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2fkcllgdp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2aiotfsdh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2nokchujd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2pmjthjsl.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2jbtahxew.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2dcodtkqn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2zgbrkfpv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ivhxdjwm.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gakjpxek.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2gdzodeat.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2cwnwfwtt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2lqmpadgz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2zfgbpfdh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2vviyibwl.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2royhpyzx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2eftipiko.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ycmeyorz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2alejulmi.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2whepfctb.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2finbeiuw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2snaxivco.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hhwisuxu.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bfbufzaz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hdaahjkh.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pcqewodi.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2eizuydma.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2gzvufkqq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2itxgqwrj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vuhertby.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2hfxqitqk.html


<!-- 参考信息 -->