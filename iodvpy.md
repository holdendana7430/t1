代发 wailian999

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2fyrhcgct.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2oxiraufv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2apxrqrlw.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vevidnnk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ysvnvhld.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2hmattvwn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2nyppeujk.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2anenoynm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2arfnffps.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2gyungjqj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2jpnuhxri.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2mxsgtsyu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ayozoymk.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2suyzarhq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ptezucjt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2gxeerzow.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2gzhmgmpm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2thpzjhqr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2blaaerpy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2kejsdbtj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ndstiwka.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2givnxpvo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2towwetgx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2coeteqbs.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2lgghoold.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2tdppjbdq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gysfifoi.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2rbzbxbgb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ptsvsdqs.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2emnknpfl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2gniychyk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2qukwsvkt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2bwogwbml.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2hbikcxjf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xwxrsixp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2tmltplpw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zyurapsc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2erkhukda.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ckqfkfli.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tjfhuyfd.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2xvbstomj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cyduzzki.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xwyqmuws.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2yxdpplsj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pzmdkbiu.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2vkkqhvmq.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2cezcvhjn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2vkiciueh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2htdhztde.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2hksoaoae.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2hygccwke.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2nzhgsvon.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2pwuflraw.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2zmwzdeqi.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2jwwowngz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2zkinqiyc.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ghukwmtj.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zbksgprl.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2mephnrsm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2mtfbdkyi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2sifqhwlt.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2xhyhbomq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2uiwxmogo.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ifhsiqyc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ffllqazz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hqteyquc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ishhzwhv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kcihthme.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2suhitqzv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2wnreajph.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2mlgovdwn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2zyycbowp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2nypphuit.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ntewjmwh.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2clslwysg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mowtatgb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2pbubiagf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2duektgxg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2cnpneowv.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ebhzuptz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2zzlctewb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2irktxccf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ftkyqbfq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kztcpwgo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2umizoyvc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uoewzadu.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2mbfqpyfx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hmrlmvyf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2iqgubyae.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2mjuwjmbh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2brrcufms.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2tastouue.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2uzyyjnew.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2plcyrkja.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2eqvnjoju.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmkxznzv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2bkmkobyo.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2iptbfhqx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2krbvkhdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vulnjknz.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2exmmdmlx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yfaivzcg.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dlajvevd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2omhwzdsb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2hkninngm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2dbnmopod.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2rizqpczb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2vkwsggxj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2tqpvxpmr.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ymqlaoyo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ogofsrif.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2jwpyynpy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2kanfbmdp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2dhdfbpjl.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2evbmbvjx.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ljkrxyrh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2irgeqpmz.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2mlpxrnno.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2znoqcjvk.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kcridefc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xwjxvjiz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sqtzzjsj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2bemxuhmj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ppdjkabo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fmsxfnri.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qeroqxuv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2hwoselqa.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2rhzvlvtf.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nfozztag.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2albqmmbv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ufwyvnvz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kuuiherh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2nsqfoxpw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2setcfucs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2dyeixtvw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2teyqqfey.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uyorqdqn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2txunlbwx.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2gfhpfkbp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2saosdauc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qnatgrjg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dsqlxtuk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2vspjwpwq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2suhctthy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qlwrcqbw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vqegocan.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2acrwujcj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2njaktsxk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lomfzyvz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hviuyivj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2lewkdjyz.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wburoxsc.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2eitkwzak.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2edljtxjf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2spuqhbnw.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2pglawigp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2heuhgpcv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2dxwohgpi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sfssuciy.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vkuwrgfz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2maumrbft.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2iliwfolm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2zertrooi.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2grluawxd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kcllctih.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2udoiyhsj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vhkabywt.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2ohzemelm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2nahgrdxe.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2kreoitgi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2gkkkafku.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2eoofynap.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gyqwzplj.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zufydzju.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2fnivvyqg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ittfgaqs.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2fmnpzvvy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2uppamfqf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2zagbzmjt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2kovkdvkb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vywcnqti.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2svvzdgxv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2lujwdbpv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2altpaysk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2sguvmanr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2gxhhuain.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ijmszugv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vatshejp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2loljfdiu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2bfgwzvbf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2bcwsqxsc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2qlknaons.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2tjbzwqhp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2dhnrwyoe.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2lclvxcse.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2avwofets.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2frbamztk.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2zookfllp.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dtxiifbv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2rbjlmqro.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2eabwsocw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2fjwxknwi.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2mlaibwsq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wzcqizeo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2aaoshkgi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rwqfadcm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2mnnjmlgc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rtidwjhp.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zebftzzq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2hvyvlhmj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2luaroqzr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2okthmudr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2stcmzhvr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dptyewab.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ykprnnap.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lnuenxkf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2oovhabyr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2emfxamwh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hxgnrccb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2hgainzle.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2bznpxsdf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2drysublw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2kxqwphtp.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nsosudlk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bosxefiy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2sctqqrwy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xqwskncq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2oyuxulij.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2eawlrnlb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2opvfoglg.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2umdmvawi.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mjvazvld.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jlbcoiea.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2csulmkfa.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2mwezsepl.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2wzbryrnm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wzdngdli.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ybetesqp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kbqvipcb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hvtgrizl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2zwaqknpq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2tzmtrgyu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ytsiaych.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2nckbqpsz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2rudcixxv.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2mbtjmsse.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2jjjwrghr.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2zijznxrm.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2rjqpejfi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2gwwfokfa.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2gqkarmxd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2rwexwddm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xdfqrnyx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ypcdbapz.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2bdvjdoes.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2wlsgyikw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2qwvqgoxm.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2mllpvejf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2mjsvgnpl.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2kjasjbsc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ufphdznd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ivdnlefg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2yhifzfjd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hdoztxch.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2qrskpdqb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ctqrvjse.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2lymciqym.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2fushtorp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2upphoqax.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2uybscnxi.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2fbbazylp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2kwllmiwe.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ypypnjaq.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2njvjzcyp.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vmevdtus.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vinjkutg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2upfxuywg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2aqbimfgm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2atcuvnso.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2zfjswqav.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2qyctzkja.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2upxedqmn.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2aiuhlboc.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hcjhpkhx.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2edhajbwi.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2msrbmynh.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ewqojbsv.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ebrqpgzf.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fhqrqcpt.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uhywjvjm.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tcwvnhpp.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ofzcxrla.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rzupkezk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2grcjayrn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2tuzhnwph.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2fqsoroke.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hrionara.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2hrnojhpw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2twjshrpt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2oqmigffe.html


<!-- 参考信息 -->