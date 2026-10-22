代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2atqoicfv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wugvykmp.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2oanaxjqo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgvnjpla.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2idwsdqvk.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2hsngwbjn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2yrsihmru.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2stkaawaf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2useujiee.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2tfnmkiga.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2wrmxixij.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2qeiptwdy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2dhpfnvrn.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2kumnlned.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2kyhvqrnc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2hnghkmku.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jrcppnlz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkqsntvz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ebqpassa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2qvmjhadb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2vbwuimex.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2khcaflae.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2pvjaepea.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2kphojipf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2qcgifzai.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qgboemab.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2uoqsrdpi.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2pdixzhja.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2yuqecrnm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lrtqunpj.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wiazegkr.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2onryxfjx.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2tediukdg.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2nlohjorj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2qemoabim.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2pbbzlfih.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2pemvgsup.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2tbqjadfc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2gomrxhyc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2vcoddnkq.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2jkuilqkl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2baysdcmz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2stqfpmnv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ttwntljn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2krnehsto.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wfrvafft.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2zonxgizv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2gwbtlgjo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wgyyline.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2hkyfopvc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2cmlzgwhe.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gefihxvs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2evplltrd.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2vdlijjmr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2xtztuzln.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2lpumulud.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2alheuvbj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2kwevjraa.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2yicgeqsq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2wbgyuzdp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnwbnlya.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fpmkohxc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzbonblf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2zslqcjoi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2cuxiqhxi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2gbqqtgwn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qofzmaim.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2kdftsoxo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sbegnafx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ermhneae.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2dyaaesaa.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jlgactpy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehicykyc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2biaybnzb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2omurnedl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2gzarywlh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2xzckltth.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ngvjogwl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2pdtqgbcj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ixecvdfq.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2liyecnet.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2glnnbbkc.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zvtdqsfb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2iaqacrbo.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ipreyhox.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2qqfkyjsx.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2pldokqxi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2dyqzumzf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2jebzfxkr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2eantrwyh.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2qrkibmnp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2oeummncj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2fdcpueec.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2zeftveas.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2zvfjpqis.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2fyvlghnh.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2loukivxa.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lowpnbpd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xchmdlqd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ikxpfyfm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ecyetsxh.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2cpbjjnyd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wqlsvive.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2slkdgiwt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rgflhjjc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iydyqtyt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2csgyiymz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oucevgmn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vvnavjdz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2vxhzqjud.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2hibvzxtp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2izybdpit.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2vhyrnokx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2wugcaxqo.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ilvyhmmv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kscqizfy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibfdqdxn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pjqcsgdx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2vlejfisw.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kigxwhfu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2zbmkljhq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2xtjkaasy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2jxobfacl.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ftnxknwr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvsscdhg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iqunagaz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2xqegmqph.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2gvcvrrwa.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2hhbyvygy.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zpolkoue.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2rqivffhp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2cktakwni.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2uaimcwhc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2gzpwzgvj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2bfdvrzqx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2rzekuubf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2uhikipzf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2uapkwpys.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ahtaqndo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fnhxfjel.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2lgutpfmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2frbrrrwe.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wwnghjkn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2fjmjqzax.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jhimsbvt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zfohayjd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ahabceqm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ewoynjlr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2oxpgyvph.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2plebsqgi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2lvtrhzuy.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2zjzolves.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ftcgixdc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2gfhhaxtd.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2grcoigcw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qmyrlyam.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fkrmxbtg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sqoyjfci.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2analedei.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2riotpcsz.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2mxzxlqhk.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ctidxigz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2scyqyzdw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2lnosmocj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kvdpsayj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tfiwwqsn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2atxkjsmt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2futwumtz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mgwyqvzj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vydupsmr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2tvgqrpkm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tpdktsjm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2mamkhqez.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2zftinybb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2spsvgwvs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2sfyoznag.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2nomttlwp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2whccknnu.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2bnrdofje.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xkfzqupo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mzpwfgra.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vuzdrgcz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2mwkrkrew.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2tehhtnaw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dzkwxhac.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2oydbqwuk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cdmswczv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dcdnbdmt.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yoeejcgl.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xqdwusvu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2hlthfijb.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2racitzes.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ibosmfvt.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bfryjwyz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2yjyolsko.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2xesaahnh.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2nytvsmhc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ezphqzjd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tzakevzz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tbrjqfeq.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2sayledge.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mlxfdtmi.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2vsohhunh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2yihlmsrh.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ejpxaaxv.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2fpcqdjqq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2yehlgeny.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2mcwqqdqh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2htduxymf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2vwrqkjct.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2xjepuync.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2jjyswzee.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qequphnv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2probpcgb.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2lgsyjlyz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2fdifwybo.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yiccehqv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2kxwxcewp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2hryfykgw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2fjdhlrer.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vqvnbfts.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2shitnwcm.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2wycwlixm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2zxwosyxp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2vosznigi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2busjnkox.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2fgjesunr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2mibrnokd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2tyzsgjjr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2vowyhwyg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2eqsuewuh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2tiyezygg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ftiyzxhe.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2fixwsdzb.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2lvzxpjwg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2bynrfvzt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2zvimflru.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2nlvryavd.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wblqjvfa.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2txwyfqgd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qmokldmp.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2gnxrxkqy.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jbwooifh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ladwfzri.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2emivojpq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bspqhxpw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2vszcblzr.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sbovajhh.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lepkzyoo.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2gjjqudbu.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2zkclehsu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ssuvqvfz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2siqztflg.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tccfcvyd.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zngwalmi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2lvastwrn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2jonziulm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2opprplbd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vomykxgz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2zsbcbgqc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2akyodpnx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lxootdim.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zzfmryhe.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kfxzncky.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gdeqzkpz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qfltzeaz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2covgsxqs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mvhlvkcz.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2juyvqold.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jqjbhapm.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2sohmxzli.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2iyfxqvuf.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ouuvhmes.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2obtrktcx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2chsvvexx.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2erdefoyv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rhxjojee.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2miyopzha.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2olrbgycq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vpctgjny.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2hmmggdax.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jcjxplet.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2grnufyqk.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2mtlkjvsd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2tjkllrix.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2wunqibdp.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ascdxhyw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ruhidebc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2zdzaiblp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xppnxdhm.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2jbqwdrmm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2uxfscxun.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xssjbgbs.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2tlupmxff.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2thvktokw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2gugmeera.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2qxtjbwva.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2awemmqup.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2dnefiwuu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2shebcldx.html


<!-- 参考信息 -->