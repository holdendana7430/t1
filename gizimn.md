代发 wailian999

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vlvsbxjw.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2pzxnbmje.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2jfrhfdzs.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ndzomdvm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2llzluizt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gescknsw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xxnfaegx.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ejizxccc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2njxykkta.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2pmxzzqgh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2lmunvkiv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nizdgmek.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2asafzpuu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2nvogwpla.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dhrqvwer.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2fqhjdssp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2tugguowh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2nycdqwmr.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2hcegvyyg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2hkoqevqo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntdjcmlm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2acpfssja.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbnditqu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2hhegsyrq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2caiqcpze.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2zqjhjobu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmgwzwmg.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2giuinpzg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nbcprncb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrszvmho.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2azzinsps.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mcuhwava.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2cdodkhsi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2zchzvyia.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2dxtuclpc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ynxzkjgf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zdrubfgk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2zfccnmdc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2rboflfrb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wrceopkc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dqmujxig.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dpzujwsy.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lntzrwwe.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2cuhodkbj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jtftudkn.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2tsczixff.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2jkvqcjtj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2edngogwq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wqyibyzf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2fmyiznxr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2xngxprja.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2cwctyyts.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ihlhkwvb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2exmvxmmy.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2bqlwcnhi.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ozzaqktd.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2esysunic.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ainofvwo.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2sukwlpam.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2rjgrxxzn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2wcgnzypf.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2jsheskwo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xqcirzzb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2erbbtkoe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2mikcmhwi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fsvcwndu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2urruygdj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wtxetaaq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2obemseed.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ayebhncc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2fvduowfs.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2sohtekmm.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2twnvlaaw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2dqnweexa.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tsuylfva.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wffslfys.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzmohuzx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ayjanvrg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2kutlptoo.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ccxqpeas.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2xpjsrfwd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2rujrjptn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ioxcbkfk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2rlxutduo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2xitqzdbc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2mgkghnyg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2tuwdhvgj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2cxbswslr.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2pekclzqw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hciieich.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2phzkldpd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2yunbcchl.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2qsptlcgf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2vgxnmkbu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2rdusmqws.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gitagvun.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2nanrwpif.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2dfmjiazp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mrdzoqqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xolduxvn.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2nqbdudse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwwegymy.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ivhkfwtw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2bexiagza.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2udhcxoxx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kziqldpc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2bfsbrtex.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2gkzydhqz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2mxgdimzr.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2dcougcch.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2snvlgopf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ytdlxvsk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2tbkzfmum.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2nhricgdz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gmidcxim.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2onvbnutd.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fbfgeosg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hzbwkurm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2lhfwvimk.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qmohcker.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2pnivhlgs.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wzndbxjt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ibsziugu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ickhjwbx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2psdvullv.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hzbtokwf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zszhohbu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2snbsclaz.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hfyfnkdk.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2wvjydgat.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lpzrvofs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2mcebfuzv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2jpphhuay.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2tyljbxxd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ycvxrith.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2rtnnwfco.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2azrsobsw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2qwdlfvpb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2cyucbbva.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rmxczupm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zxhmhhjm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qejjnptw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2cvwmxsnn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2mfkcfrwu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2kvucodta.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hbtuvhnk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vxlgytmq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bpuwfagf.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mxqxtgbb.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2abyqexho.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vvvihlhv.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2aypocpjf.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2xxmgusqe.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ilddhweg.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2uibqnnqf.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2dhdjllxf.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ldkwsbny.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2uypyqmwp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nexymmwh.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rrmqqakh.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cjytqszf.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tzxwpngx.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2fmbjvxpa.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2bjmzzqub.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wnavhpym.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2xgnpeejg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2jptmjnje.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2qkfspqwo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2rsbgelci.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2nenkhbhp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2tclsjpwk.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2bbiehabw.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tktplbqk.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tennfnjg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2bzhryqim.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2sodifldg.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xxqczwrv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2tmwcdebb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2juakddnj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2sgywjdtf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2pbvzwhyt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yudsvmki.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2zkwjkmpv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2xfgiafnu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2snqjizdq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qmeiplfr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2nxdzoddd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2uqfvhpmx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qwpjulwb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2mtpiwrcb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2dvlxdalq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2yiabzawc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2bniwwash.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ylmuibvf.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2oyjcqopt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2exvmdvbd.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2htgemxbd.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gwcnmfbr.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2lmlfykpz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hjlgyuih.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fuonehia.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2oloqdgai.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2iehlycli.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ntqsimgk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2magcpwqa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2piswsuul.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2thwrroio.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rzgjsogr.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2rijafuss.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2xlotaubv.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ggeqaakj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dhrgxpkr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2fyzssfis.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oxaqpyer.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xziyfqyy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2kbspuptp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ocatcmwo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2wrnnhiah.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ynexjzmm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2cebioayn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rfvidnqj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jbgnsirp.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2byllqwho.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tgmwdozg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vngewfjb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2sublgfnh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2imdhghut.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zwrmucav.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2xutpbxwm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tppkfrog.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2oktwqbbf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fnjzsera.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2grnziurl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2mzundwqv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2swyuolic.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2owbqyurv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ekvrbfci.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2drwwkcaa.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kszdpuxs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cbfouwlg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uiwlbtev.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cwnyxxqx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2qmynuikg.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2jcjwkxox.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2rsqezxga.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2gbhqlzxa.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2qpvbzktn.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2bubnnchp.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2jeltdmbw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jrcfyuev.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2tlgnpbgh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2wbfjsujp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2negdzxgx.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2yponpzkm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ionmvroh.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2oixwjvzp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2bbsafsme.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2tvryqcmz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2yjxrhlry.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2pglfytdj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2uslqxayc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2arqbdqwt.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2qhssecou.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rxmruuhs.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ggcsbgok.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2huzkwnjd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2vkyuiwur.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2uztobhrq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2yaxkotrc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2wmjrekqf.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2pyqzlpfp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2jlnlomrd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2bzdskelr.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2zxfhxwtl.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bsapvfqi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ogxxruah.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jrcsaxld.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qlnipdpa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2wsxwkxsl.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2zecqlmzb.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2znetdbgw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ggzxdpwa.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2gncqxaxk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2vlujalef.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jekzpysm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2izepbqch.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lshxosnx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ekboxlea.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xewnhghj.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2teunitls.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vuazjdjk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2atwkmwov.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2djbkgtpz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ibgfwfmz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pwsbsnvy.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2nhgpafzy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bmgoytcy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zlurtydm.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2vrvyweui.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2atvzvien.html


<!-- 参考信息 -->