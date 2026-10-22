代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2jpeopdyb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2huncvbmc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2tjtjcllm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2szddzqzk.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2giyydjnb.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wjdejzqd.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tppfuuse.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2wokdddut.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xxbavntr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2omqjffcc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2gnlitcfo.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kysayngd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2gqizvynd.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gjezgcyv.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2altlxzyr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2suovimdc.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2gmebxona.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2kesmjlij.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2qethbyab.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2scnzahlw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gouqoxgz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wsxpateg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2zazbsjod.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2mxlbjdmh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ebrbnlgv.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2blafnnjd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2cutnggwi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rdnqhflh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2xbvphgis.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2qcvleqaj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2pegzayfk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2dnglzxtg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2jrpzxnqi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2pijlgaig.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2xihyldxw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2djkfcirx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfzyorqn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lxrgobyt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qvooxixl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2sxlyyggt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2vbzbtdax.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2qwzwzrrp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdsdicti.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ybzgmxve.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2gwkafdeu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2owqqwknx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2kqvaleyr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2jptynchk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwhtqiok.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2nwwjnzdt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2gznirgyd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mmwmupbl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2mhqelrmb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2otipnyho.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2fhilehuk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2kzqucnfn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2oomwkstf.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sibkhloc.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2peflpljj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2olqnzoft.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nihkzuxi.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2dqfkalwa.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2hhwybwkd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2xtwxsedk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2efxeexvy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2cpsadsin.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2jdfpzoqc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2etiinzka.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2tyernrbv.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2migdlozm.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2jysvxsrf.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2eorvsqcr.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2tgrqgnaw.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2nxcraivr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2djnfwynh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2fdazeetb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2edlgcxjm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2jaiisdzx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ubfvicuy.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2afwpbend.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2rhuttziq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ingstkgq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2grvbhrmq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gdjzulcy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hgeosemh.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ruxnifnh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ukmhlhkr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2xbhzkodr.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2uwygkohr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2acjoehsr.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wikwqikm.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jfvzthen.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2uugztgda.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ryicsnyp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2jwccadni.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2gzffcpxb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2kevpzzbs.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2didoqlam.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2nthumahd.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kbsustup.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2khjiwxmu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vlrlbutm.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2kfkvonjm.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xcvtwygq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2shshyfgx.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2engqovku.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2gtpruqxa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2jbrvtxlu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2cyekqlvu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2vbepvcah.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2lhsaggai.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mceatiey.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2nragbtzc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2vbumsqug.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xoukwuha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zvunemqv.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2acxsrwto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kjqljhlf.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qoutpdly.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2xrgoqedp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xqyehlho.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2aozoqaop.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2gwedqumb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2utwuqsfm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2yliramdn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2mtmiqbjf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2blcrgmog.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2mytxdohx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2esaeukrg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ooldrrns.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2knwllcem.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2unruskho.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2msjngubb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vyzixgeg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2eornmhsx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2hyrtbpkv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2eonddbxb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fbdffnqi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2bokrrpor.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2mpskfzth.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hccrbedh.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cgyqbrpm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ynrhwwng.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2eegtgvdf.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zbedohsn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ttxtmgek.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2afvhfrsr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kyumzmdj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2onkmenpn.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2fdljolxs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2zrfumvaw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2mfhwydqp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zcbxzdim.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2rxdsaxae.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2zjabdmks.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2labvsrsk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wwqdbelu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2azeqrfvc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2oacolobi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ckaspxjk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jgmqrnny.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bubvvhlr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rikydqkp.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2rydlbhex.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jarwkudw.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jlqynlbp.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kpyyxpku.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ebywggae.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2hakcswqn.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jmtfwazl.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2hdrfazzg.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2bujbrvou.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2abxwwyce.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2klioiuos.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2diezvrkk.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2aagiusdo.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yzwihrcb.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wvzizmiy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2cjkuvknj.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2mxmmxluy.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dncclipn.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ayamegri.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vjllgwhm.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2arxwzzvw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ravlujyy.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2aiuzkmop.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sooypboz.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2auravdqt.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2eaqtavij.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gszqqdbr.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2kcfrzlmo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2pynwdjrp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ibkorxic.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2mnoyflqi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ycxopkpy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2slsrjykh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ykmoyfyx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2eravggab.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2oshptepd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2zpasrzqb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2dhnykeji.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ezkumowe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ancaowfi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uyputgll.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2pknawghj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2rnkhbloc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2zjujagie.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2jbvnhedk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2wskpfcmi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2hgrfvgrk.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dljspdyz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2dtvckkvz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2egusoxzi.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2rjmmssak.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oxgghpag.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xqvzjtkq.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2pbeqakgc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2zhnxrlei.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2fnetwmxv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jwqdjyvv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zvyrktsg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2cgkelofq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ycrnpsnw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2aubvmwjd.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2nwjusahs.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2dqrxswht.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2obyrlxhv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wswkgtka.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bejlibar.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2udobwkrj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ysxldmxk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2tbcqxkpz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2sktzjwnp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2rfbygblv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2trqguslj.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ldtqqhjq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2myeztvrq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jtlzoxef.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fhmiyaxj.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2sjybwauf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dnoialak.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ercqqmdk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ovjegrfm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tligrefg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2uwznqreh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2eagmrbtf.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2hilxrubv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kttquehg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2yjbresao.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2npdffezp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2avuyavao.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ykdyipwz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gcvgafaa.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2xuephyyg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2afgileko.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2pvgvlovt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kzdygfur.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vmjwqmuf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2qayzndff.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2pqzhnlub.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2lefqrbct.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2vjgadhkm.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gcsfiiiq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2saaamxjs.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fbubfgeb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pcxzeuek.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bykypirb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2qjafbfzh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yitniqtf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2exbwbscy.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2tgufzgqh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2dypmznrx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2cdvyjosz.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2zziylqgc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2gdjprafk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2vxxwgfth.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uouhgngy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2cdmfnwux.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2svyjrukf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mlathjff.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2xecmryoi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2kcdtzzro.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ypefmaym.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2jxeccbtl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hsmtbtgg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2cznqoyrd.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2mzlqqxcs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2yorhsbry.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2xxnzwddj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xuchcwyh.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2bvmuwivm.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2tadcuhdj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2sdpmngzq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2stvszbdn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2kxuchmhk.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2yjjmsknn.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ydzxpfrm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2lccpriqk.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2lrhouvsn.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2pwyxepez.html


<!-- 参考信息 -->