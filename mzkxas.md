代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2isecbjmc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kcljzxgf.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qrapehuv.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2tbvyikma.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2nnvmjpvm.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ssflavsc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2duuxppam.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2nwrxvtbq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2grkxwvhy.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2voucvcgq.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2zalpflpn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2uoztamie.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pncvcini.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2qkvglidx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2jjjfbvmx.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zqgpjpep.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dpbcjjtc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2newhfzbx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2hjkfzwrz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2rlghdizc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2usklntwe.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2rpvrfvhy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2pyjdtpgt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2pgpnxrew.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2fwxpgspi.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2texrzdtu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2esikxtcz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2nkcmkqea.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2ftkklnww.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2aqsocxbq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2asnzxlfj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ceexdmcn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsagyrfp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wrruaioh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayfmegtb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2eifkdhzb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2fknunnam.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ehyglnuy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2juslmcbx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2jogpekpe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hmbnhouz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycbcldhm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2hqtqfzmc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2yqebwcdv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2wvjremuy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2gqkhgckt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vqmwzvlr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2kmgkfkxq.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2tlkijlhx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2wgmtjitz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2qjwamljc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2eugokcqf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2jvgkneqw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kafhvlhv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2tcivtljz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2jptjmkdk.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2latenslw.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2aigbpujh.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2dhsqcaka.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ilsnhqdj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2canvxdly.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2gwdgwibc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2gqlebgnk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2kwpsnxtd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2zuusvlwb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2nvgrhfiq.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ymryhyut.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2zcwbgeth.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2qwkmddyx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fdiqiksy.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2lsjuwdun.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2sgqaxfaq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2pudiicdq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2itjumqnc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2tcdvpxwt.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2witdztlk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fgdvcuxw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xvdzpsez.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ekktnrnw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzrkpgid.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2apesqczz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2itnvwbcq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2gvcftipg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2wvwqweqt.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2pbbbfawh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2fvghbdsc.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ojkpxnlp.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2agtgexac.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejebpgha.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2zmocyikr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ihlbyxbn.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2orhbejzy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2wdclhezn.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ojpnucvn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2jruvrnob.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2brxmbgcn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2uifgjrgq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jlstgdil.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2clactozy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2idjtzvur.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ltppfdkn.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2nkpwglld.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2uuqnenrr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2npncmbwg.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2sndjicpy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2zgkbfplb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2wkysnmyr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2fwppxysu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2oentxgbs.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2flyukxcq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhbctoio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lujfkbya.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2lrgvlcxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hekwucbo.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vwegzoqs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2yxthcsjk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tykcdeie.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2fyvqqacb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ftgljfvq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2iwutuqhu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2xmvncckt.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2tfcfcbxl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2dcosrhsd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2scaorsww.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2btblqcqe.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2vxnclsyy.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yijyuups.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2rnfhvmxu.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qcjpwfxg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yehcnwmt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2rgqmhlqq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jvvnztyb.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2jurovewk.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kukroqfy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2lkholdzx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2jjlesofh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eyfsxqkp.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2avlmyxsk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2pgwshwgo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2fwdrpsjz.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mcixvaqo.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2giieruqw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ovedaeus.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2gqxjkvln.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2cdzythbh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ynkiyalh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kfqgrbpm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2iildugpe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pihbyihq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2uevwivtw.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2skyutbwv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pasvvguv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kxvhcglt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2deiljjvj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2prbwkesp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ufbovkxw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2njbwedns.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fjatypkz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2afzqfskj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2uykczoye.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zkgfkibh.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gpwhzbiw.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2litgkrnl.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2hfwrlcsg.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ptqoogud.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rurosomc.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ofbcqqxm.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2tbbhbdvq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2uyhytuvk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2midcdqxd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zhesfkos.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pfminimk.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xmamzexo.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ororpihq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2knvcxmmh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2cofkwech.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2qhzrdvof.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2yufjinvp.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qfruntbo.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2trokwmbt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2xhnbukum.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2riocyvyc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pkxjqlli.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2zawkzomj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2tdavvrsh.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nxxnlzqj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2hvsfjosl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rjobfyvr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2akcsrizl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2xyeqodkl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2syszjyln.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2wanpmtoz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ktdwjbls.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hkjtedjn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2kiexpjsh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2jioahwew.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2qmzxctyr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hxcnkosw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ahvqrvta.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2dsivyiep.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2gzpdpepb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2pfejdgeb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2wqugadqj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2dwdqrnpr.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2hizpkogd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2lvmfahfd.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gbjjfrzu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2dbcltvnn.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2njjveonn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2kinpxumm.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2esfczrbn.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rcarnswx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xopsqbjh.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2pnmmlpkn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hcnpcsty.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wykspiyc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yachzfdb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2lxrspwqn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ddnvxioa.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xjntctkq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nbpubbkv.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2lthqerxs.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2fuuwnagq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ibpqofdf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2bbdebonc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sgxeehld.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oblpflif.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vtjosfnb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2piuragke.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2npfdltzn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nbvjpxme.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ehnqapjf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2xmqvfpiz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hffsdmmt.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nqmyhylr.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2upoijztb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vdzluaze.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2bfxfjmvv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2abjytjhv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ikytpsej.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2syemwpnd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bwevzzbb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2smivzkex.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zbwolbfi.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nyjuprdy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2gxlokrlj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2tupnvuki.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2genoekwz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jutngshf.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2xdirlbql.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vgdqsyfq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wbmewgcl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qxfcjyhk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mwnpbpng.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ismrbyfu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2wetqniif.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jrnymxko.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2stfwzgww.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2yijoffnc.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ozfefzax.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2yvuawgni.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nkbnretr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2wjfmtoej.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2aywstmng.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2bkzmkuit.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2uiiuxhbg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2fzkayxiu.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2valvzfbf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2iwdpbefs.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2nuwytexb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2zlgbbodp.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ptiuwdst.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2kgyjivdp.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2fszydlsi.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2kgcytdhv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ilziovpf.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2doamkkri.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tzajzhwa.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2vhtzximv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2myvxwzea.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wysfulex.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2mfehragr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2oljlflbl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2owdwjsns.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2wlatdqoj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2yvcaaydr.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wwhhfiev.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2fimnjsyg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2zmijavna.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2aidpynio.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2wtejdgux.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2hdmcrhvm.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2pmjtlnwg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2mcwiawgr.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2hagnsoao.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2jtnzcmvw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2hcxsbleg.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gdqfqooh.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pjuekiou.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2djlrizid.html


<!-- 参考信息 -->