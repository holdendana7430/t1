代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2fyaxsinh.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2saseaxbm.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fvsrcfoq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ridurtif.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pvwiqmil.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2vupxomum.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2cdpmjbhk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ivppjygb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ckkxsgxx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yrnmvqee.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ltslqxjm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2gaiezgvf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ztejfvgi.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2mayswhav.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2catnfqee.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xpvkdxlw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2rztmmmez.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2xygirrop.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2azojkeon.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2qfogbhub.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2cvxjdwqi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2cfbkfjjz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ccfasznx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2hvwljqiv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2puagxblr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqzdhmod.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbmuwhpv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2xtxzaled.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2xtkjsrxd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2clybsrck.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2abaqqemi.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2hkeatrtc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2lovphgre.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xbzvfuxd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mlbkcqyi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rnszfjaa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2bwdriiff.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2hwhcyhnq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2dsxdqfcw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2gvtraxog.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2tburbcnw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2fjznocqt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2wkynpxjx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ectdvtlg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2hdsjrxrj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mlvrlpes.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2eyyqrret.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2qgjkqojo.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2djcqwofh.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2plhoaces.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2knsxlyae.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2wenqasgx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ikmfjmod.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2xuwxiglm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2avpfmtgl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2rgbuviqp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2kxxniige.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2fpxldpzv.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2zuzjplbp.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2qznwnbnk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2nhbwrkna.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2pkihkegk.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2izeapqvt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2xutpujhv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2irhyxbpg.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2dgkdvjbz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2euyhidui.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2aznxmqjg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pczkzrxr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ysfdtaop.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2mmuodztk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jigevjue.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyezslts.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2scdzyopo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2mgtefchx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2nymhshyp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2pqavtxay.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2uewpeshq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kzegiqig.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cqkwqvfa.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2otzwybci.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfanyqpg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2lztvzbhk.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2egkqqtbw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2cwkjryuk.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ifyzlnjq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2iglpqbhi.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hqndujih.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2wkjoxrll.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hapikdvf.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2evaovuyy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2blrzprmp.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2jbdhsyan.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2qaoeoxki.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2jmwxstov.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xoiozyyj.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2zgtcpuox.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2nbvarujt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2yqwfbozw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2btvajpxm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2cvtueanl.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2pfwyhgwj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2jqglrxix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eabxnnvj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2wmrkoghp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hlkhishx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wquikmeg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2oudqbifd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2yezhpwpe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2cuqytinz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ptcugfbc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2gniyulfz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2kdeojqly.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2nhjhwiqi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2wqxpxwft.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2vpukcgte.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2drgpnrdi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2fxskhgnq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ojsauify.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lvfqtdgw.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ovpebmbb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ahkegsld.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2nxiujdrn.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2sdgljizl.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2epzlxbuk.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2negtrwhk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ltjzqbtp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ghxkedpn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tbketcyk.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2woyxbyeh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2rzladvij.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2tgidcglr.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gvfsewhe.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2zbapnmqu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ftqnykyi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2vizbxook.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2kmsdeunf.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wtksymtp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hbixnqlv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2mcppmhsj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ueeeixlo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2cgghokcg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2xdxrlxfh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ixwfwnlv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lnknpxjz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hahbkczn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2zbhfihjj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2mwgypasj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kguqawdj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qbnlfdne.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bszbxfqa.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2meebsdkp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cwzuxsxe.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zptlhsev.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2umkanbbc.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2hmifsrxr.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ihupplfr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2iehwipym.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nvxvaolf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2dfychbtw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2vvplzmgc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2aetbrsbe.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2urwrqhwu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hfaypevg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2glefjiqk.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jumavjhx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2zycqxvew.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2efyoaith.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2viyanjcn.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2upnxzptn.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mmnpjjtc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2tkperldk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2gttwdasy.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2muwrpylu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2motelxql.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2joucsiwt.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uwdhmuia.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cijbvlwc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2omczorgy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mkunzskq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jninpsja.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2twdtcuhf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2qnshfdkz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2axzswbtk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qxkwlzws.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tkavzbwo.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2bncevcsd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2qwkwqfjl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2bpgckiba.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2awsoiakk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2aqauookz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ikcppnhs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2fzdutaps.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2vwpqvyvb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2rauxzydo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2pxamsyhl.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2amljjttg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2onqwzbwr.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2wfgxupaw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2zlcrpviv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ltczgefj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rsmkbfez.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cwcepfir.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fphssvgn.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2mmonjira.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ktjxdaru.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ueriycpx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2yizxwayk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2paxxitjd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ocxbzdcs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2hpuidvlb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mhmpvtbn.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hagxnwoz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2nujjltze.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2lxiuwpeq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dcggqpki.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dllcscot.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rbrruslp.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hgwqcfyk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ynduodzj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2bnazvedu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2rvdorwfd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dgqzffhx.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2grjrxiar.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2zjcgozjj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bpbralfp.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aedjngfi.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oveeyyag.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2bstwcohi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2uadziqui.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2aexxewmm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jxwefrrk.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xhnaiaik.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kmkwsabr.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2vayedepd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wcwdltjt.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pezyxlzs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2eizpioqm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2uogvyvtp.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2tlfbsfmo.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2rlgacvll.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2vneiocfo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nytofooe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ajindeuv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2pqhnttov.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vjuolgyp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2omonhdim.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2utbcwsiv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2atatdtmi.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2aapwhfrc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2tbejeors.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mqboihdh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2yuawyojz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ellncicm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2clvakpnu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hfshnfcz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2hdudyjyt.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2guqkrlow.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2lzsdqylf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2fqvhcduo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ihsuyrii.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2zjltmbdm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2kzwggohg.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2hlroaqps.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zmnoaowm.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2epwrhuee.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2fkyzvgnc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2idjnjjsy.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2tezagogq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aafrvvzr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2lxwrzhil.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2iyxciids.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kslcuacg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2uuonwant.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2tymqgjdj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2bgehnorg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2tifvwktn.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wcsultli.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2gshvhlum.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2odsdqmjz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vkdgrxug.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2mtalkmig.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2syzzdyjr.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2nwhacexg.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2klhxsbev.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2weqlgdfs.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2munrcxrs.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ozcmlzfv.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pzgyhjdr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sqpukzsg.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gtozogzj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bairswlv.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vbxvswqm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mzvkswvy.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2emfsghbt.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ysbdpsko.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ezkjxxlk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2hkjlfpqc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2irnllvki.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2btitokrq.html


<!-- 参考信息 -->