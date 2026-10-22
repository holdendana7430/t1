代发 wailian999

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ywmjbypr.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2pwnxfyte.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2urwfceui.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2seixzwwz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2oszlrdkx.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2etpbxvpa.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2bwktfugu.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2udfjuxiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vczxplce.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ieapodlw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uhiwvcoo.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2rwxrzrbd.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2sjygtcth.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dttpsrps.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ornkmiiu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2veipbebr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqiwuggy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qglhiigz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2kvwtyhtd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ximkqson.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2mulkzbdr.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2vixegqmp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlmqpujr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2humboacu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkufjtew.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2mqiqujsn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2rrgyrdqn.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ijyysxpy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2apxjnpaf.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2fxhnruqv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2vfcpmwng.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2yrxoogqn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zfealmuv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bdtqwksj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qemdkduj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2loklmfto.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2qmrxuyah.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2rogylofi.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2bsemjrlr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2qbgnhroa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2zebglrxs.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2aorkryep.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2coooouus.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2dgorytnc.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2unkumdce.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nvpqtven.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2bgzdcgon.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2vgcflpxp.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gugldsts.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2kmcdlftc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2hbncplgx.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ursmqiix.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2rurasape.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gzdecmoa.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2qrzherec.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2shgqfrkc.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2vduunwxq.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2nbazbfhv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2zafwkzmb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bzaztrgt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bkkaucpp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2aruwfnmk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ekstivmh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2airzueot.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2fpfcbsfx.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2hypzuxnd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2nzzdgbsc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yystkyfq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2whejldox.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2xfnbhtja.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2pxkusrvk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2uvnbqqrr.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2ztrbnoam.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2qgmiicsi.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2bxkdqoqy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2jgzvzlsw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2drrxblwf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jruidwfo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2eztvknqw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2mjjvvyxu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ubqrngiz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2hygpbmmm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2awbacnzk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ejjtpwpt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2tsbqgpbr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2aiceudta.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2tywbjjyv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2siivkjip.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hifqkzav.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2idjiipeb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dzbwgupa.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2faucqcmd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2wukawekj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2dupaujcj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2yaqkngtv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rzibymdo.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2wpiarjvc.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cxkvsdnn.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qdvmesfp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2txhuwqgz.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fmedcscb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2zsznbkpr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2gjmhpugo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2hqfyxymk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2gwypimkp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2gyglwfyj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2zndngbfr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2nzlyaquy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2lpufhsui.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2lrpztjts.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2mvrmcjth.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2lmrdcxmg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2rqwctvow.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2crkqmswu.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2wubfwppa.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2kravbiao.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2zbxmyorh.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2gbtuoqzk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ycdsvdbx.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2vlvhxfcw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2avmxhsdb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tytsygbc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ljwbpwae.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fytnkyxp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xiovwgsa.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2owzwumht.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2tkxkakwl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2balqcpxv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2stdulnhi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2odyaxxca.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bjncbeyq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xwrbapny.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2poodiwrq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ygiwabpb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2cqeqvkah.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2smfjjywj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2duqrzosf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ylnnbbcx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2rsbvwdyk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2kqajzjrs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lqsfehid.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qtfqxadm.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hutygxix.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ahjwkxcn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qiqlyevc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hsaespiq.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ldrjaofa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2bscvtatq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2jxdwogkq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2gcqrtyrp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2svbqnvkh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2evleezoj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2mugszxhy.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2jocswito.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2demqauyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lhhzglpm.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2owlfjzda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rcmcyoob.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2iavtlyxr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2anriwoxp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2shypwbvy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2npvkknrt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2vbrolwlg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2okasszjx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2irexjryx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2jvpjaknh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2gpcsiedz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2zcfhpbfu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2bzisxnvv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2bugvzqpo.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2owaiqroc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2amlywijr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ifvsodqe.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2dqcgkmkn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2seizjihv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sxcuxuep.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2robihuxb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2alygcrak.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2vkzriihf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2dlnvrizm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xkpiatzy.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qwkmdwji.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2bptsmexq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2llzpymuu.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mmdwgkag.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2oicxwaed.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2bpkbdfao.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2etxmrexo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2aonelqmg.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2erefvixm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ftqosnme.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2rjjriulr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ekayivyy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2rchsabjs.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2vvtfhrkd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2atltgsps.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2plzefmen.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kyeetapa.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2dypnciqo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2lawuuajf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2prbsiodp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2luivmbvf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dvuvahow.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2uxilagau.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rdglsunf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ulmojpih.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wgjbvoxg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vzeecfzn.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ukaoldbe.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zkhpxvin.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2tvkyfvft.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ywjdvyjv.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ajvtudzb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2wkghpraz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yfghvlep.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2odvzcrxt.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gdbtihtz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2penvhugr.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ydugroxh.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2sbcziazr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2amnqukfl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ghqamopt.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kufcotqb.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2gurpornj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2yvywqnlg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2weuxectj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2vrvyhsgj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2haxwpadd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2adhpcfkj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zkrxmipl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ixujtzwx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2fitslfgh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pforsbpj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2erosejri.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2vcqmpgpg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2xhuzaueq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2oidadbum.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2fuxodqaj.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2jmemwuek.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2dbibwpkj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jidayboy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2illfdpil.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2iporonhz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wdgggfnq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2fwtkduta.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2xygkkmwv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2xrklyedl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2krjjbwvw.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2kgoqlxqc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ykrsdgsb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aroeolid.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2hmcdltlm.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vbarjvjx.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ioqpjzeu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2rzcwbbcb.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vmuobnpn.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2dtzbhuqs.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2nyxwtnsc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2cwxjyvla.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2antfztix.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rwglvzkp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mxydqgtn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2qmkxnbmw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eaftfbgt.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2rosjepzv.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2tjmbhwrf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2jhuneymw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ysrrkfdz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2oveqqybf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wdafhnad.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dnutgbfl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2mgwbrfxb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2tlzpwnck.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2nacbkdmi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vrkvxwnr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2olffrbgg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fsbermzy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2jracqnwr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2elwejhch.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mgyppffp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cxstgope.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jfuyqnak.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uxdcsgek.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rpheobmv.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vkybqejj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2oxlbzxtx.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2uqdzyqec.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nnahfrcg.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2essyztnc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2nuxuymho.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2phjuzpgm.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ejarzryk.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tqjleaif.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2cldbrccs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cuddsacd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2submpegw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2byciflnk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ulslstil.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ejmisqzg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2lepxpnyj.html


<!-- 参考信息 -->