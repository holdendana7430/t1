代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2yvajrynq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kyhqxxyg.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dzwswvxk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2xvkepkxd.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2mrdjwnlv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ldidgpex.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2yuxedvuw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2scgskmth.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2emgipkzm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2imxopuwb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2aqxecrez.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2aeymfdzu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tbhmlsqt.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2zyajsata.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2dbfofhvl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2csehqlji.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2nsywjqwd.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2lhcwfhpf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2lcimeytj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2qnwqslxe.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2hfpnzkzv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2mmxjzncq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hktqekjg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2qzhwfjko.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2yncegtth.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2agdyolvt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2saprbhvm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2pqvpuxvw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2wdouszom.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2hnvabdfc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pnakgzjg.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ghtfuzec.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qlejijpb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2lwnmuiej.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2eahhskpy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rthoicxu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pznfmhye.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2wucanbnp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ojykqzry.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ewvgeizg.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ozuobcih.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2utpycyec.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2xzvnqhpo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gzdlerln.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xitgqspa.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2iecylzlr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2duqfgbuk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2njbapyvf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2naafxbfp.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2jucxkkvk.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2rxbxwojf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2uslxmbah.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ituwksld.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2vghdniru.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2dflotrjc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2bxdpnkwn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2vjiotmzt.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2qvvvtdxb.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2idwhkebz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2nuqcpzsn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2tzcnwwnz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2trcdkava.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ugwhdpbb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2jqmatmna.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2aksdxrvq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2xxrxymke.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cdumaman.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2xrvyacbm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ncixobeo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qgzrnfdt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2nevizshg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gxmqvjfp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kteqvesz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2fdjpytyl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2pqqwuqmr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2kirxsenc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2hkpjvkij.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2dauhkgup.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fdhreuhf.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ruszjqap.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2kqeobrns.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2sexumeai.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2hlvagidu.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pdtjesfm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2oiiocuag.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2oubyempo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2qmsajhvw.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2fpsnfven.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltdwioni.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjclzwcw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zdbrxhro.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2yzjxxvbu.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ugqrvolr.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2cnsebkbv.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2jxarbgxr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2oqdltpvr.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2txsrpnyp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2faqesfeh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2kstornrr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2geqalixk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2rpaegyxm.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2rlibifnw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2hqzyyazv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2svmiqtml.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2xtwpjoav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmnnzyci.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nkltfxzp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2neuxxmya.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ywekjwbf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2gnmalepv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2dkskgwwk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2oavvqycb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2umadprog.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2cjljputx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2jpdqdqgj.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2femuqtyd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2gjuflume.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2cvesotrd.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jyfmqnfa.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ctjmuiau.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ghecrhzo.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xztkmrdb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2dwtwwqft.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oxpasnmd.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ykjrxpvu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2efzmgiee.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2mzwpxces.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2cblxxbyv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yebporxq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zufshdaq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2fcpahmex.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ntmwgpeq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xidzvhsb.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zlszhevo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2amlqdhuc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2jlyeadkt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2uusmlulh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kcdifckp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vtetihfa.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2dijiupgf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2idgiwwvw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2zjqoxasm.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2gypppaxk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gsbmnkmh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2aaraddcs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jllzfyyr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2rrenukgj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2qthbanfk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mfwmvtqz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2evygzvbk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mpvvdpxa.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wfmqhjcx.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pkjgrxoc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zfcabrxo.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jqxyqyln.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2sncnemcu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2wmzcsbtz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2krdmstlr.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2gdaeoweo.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2wudaxbqe.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2fmtiklpy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2xhqdavri.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2inokbelm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fttoyowb.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2usifkqwe.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ruymdjxz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2gcnntxbd.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2wkdwpqkq.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2egcdbkhk.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2hygmzuzv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2zwthwqxd.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2mkckorel.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2qdpktlgm.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2atksoetk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dgjptcqm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2inwosslt.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2uwxawzhb.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tzhyievx.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2wbgusjqs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2twcvsyme.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2zoyqojzn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2hvgpjxov.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2wpuortei.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2zdoouebn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mdruhxsa.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2pyntylux.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2cugsctsw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2tixixsnn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2jgyuadmx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2oadcxmrq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kbbygspi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2degiobxn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2wcsushkh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2xxwpcfgw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2htazdmgv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2gkoqhkqe.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2yiboozwa.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2zikotbks.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2jzqymhpq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2clnzzzko.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2edvwnegd.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2wjgstjxq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2akweecva.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hukjzyqw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2weemabud.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2rhwsrkcm.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qbzlpjnj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2axiyuptb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mgkhipjd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2mexpalne.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2izrkwoxs.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bzazfbey.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2pcclgwra.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2rczxdyum.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2vhnelhur.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2gawvvwmz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2crjkuiws.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jlybbkkn.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nmrqwbzw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2bdupiame.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2hevbxnnv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2xgusxdnc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lvtdvhdi.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2tymsqavm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2qokanlxj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2igljsers.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2uqfyxzmm.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2igvgkwue.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2pphdykpz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2hqhqxxxe.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hvngrqzl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xgvqmavp.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2tocdynep.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cgqkluvl.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2hipcfqhc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zjwjcxbl.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jctngakt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2pvybkjvu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2fniskpss.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2sytgixke.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tlwqvszt.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2wgroarki.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zyxmchbo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yimzcybr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2lpxudzqt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mwuftgad.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2lnmgayod.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2eecfpmsq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2afvizmpn.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2deyqntcd.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2bkcdtuwb.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jzybrgbl.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jzipqpmz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ylvzsocl.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2hyxjjotz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ddqwjhkl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2yuatnkmm.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2vvlkkmxn.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2srqainwq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2onehpgeo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2jxfxusws.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2xuxgobzg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2wqemfenb.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2vrpilnox.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fanqqslu.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2fthmbxnl.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2xgwfnhhr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2biwqgfxi.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2bcxzdoqg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2nomhuded.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2wzgmikkn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2bkhudnvd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2egjnpaqc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2puqbiuhb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2aoqsycoh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2jeqlzbrh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2jmygucef.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2jxzymmrr.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xpcfeymx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2jjodgtun.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ecdclpel.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2nxxioivx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2oxnqnawn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2iklecqmj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ptarnbfc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2pyoblzsa.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ndzkwhse.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2lzcqjdpa.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dwnoenaz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zdgqutrq.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dbevqwhr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ounuvkyt.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kmrqnlca.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qrenhmoy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2oxaxslmz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2wkuqfstz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ruotezod.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2mtimubot.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rqoobqyo.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2albtvvxs.html


<!-- 参考信息 -->