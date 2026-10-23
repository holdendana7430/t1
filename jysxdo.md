代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3mnewjndc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cnvmgvxe.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pktzqmkl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ltkguppx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3vviopeoc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3eoqjsqrn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3nxodasob.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bywaipeh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3cbraqsqp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pkqhwzwu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qjmvurrl.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3uvrypczv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fzapejij.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3aojlrfsk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3uidjjgrs.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pzxldzxx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3dvhxvsnh.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3spauupnf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3asxhdtgz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3oxvvrrgn.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3bdauhmap.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3awaaotkt.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3mokwhvqh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3wpdyydzi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggovtlkl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3oskspbtd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ezroiwhs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3zxqwlcrs.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3xwckdofu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3wzmhapqb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jjrekrib.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3maqpqkfa.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3etbbbgpo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3qtjsqble.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3fhemryyu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3nogeouwg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjrxyfcv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3vaxgmmvt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3klzfdary.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fstbvxzm.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3icleeiuv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3hfowpzwy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3hwjqgtey.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3liwvhrph.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3bmctnhuf.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rmaahacu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bapqnwyt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3rldrecpt.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bjioiyqk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3vbqmkhpu.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3enlbwwee.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3skxwfxxq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3utphysxy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3uibutdwg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3cjhjwbas.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3cwfkkcgy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ahopqvrn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3tinlqqvx.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3cphfcuhb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3wkgmanle.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3iwzexjlf.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3qilvvmcv.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3yckkfros.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3aobdzqva.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3pbtlimpw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3atahubpk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wsmpdqqm.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3estntfkv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3xtifiduv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wxuvkjjt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3hhzdmrmv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vmftdhdz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3oewlyzix.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3acbnbmut.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3tdlrkbro.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3buyomaem.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3xdasjtjp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3nvinmczs.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jqbyendu.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jayjjovw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3krbfllxp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fianawzp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3przxhozz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mupnsxzk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3xhkhvgji.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3dxmybnse.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3gyzhxeyx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qciwciqm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqfbkpkz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mudljwco.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qbvgvfdk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3kqspoehl.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3nyhwtgja.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3afmtamll.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3jdxvpdap.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3qxqiziep.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3btvepwkc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ochobbwf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3majomexl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3tepwldze.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3dibcemfi.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3fxafwrdh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3uwzzgcih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qwxlvynq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3hmzazjdo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uxkjjljy.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3pumauynt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3getvqmcd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ubkkdzil.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3tzdserqr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3pnsgkkyu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3pctxmljj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3plzmifmb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3nyhijjrm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3owlzdjaq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3sassrrbz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3exjhpkia.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3geghfknn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xzsojtqk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ooogbxqc.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3soysttir.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3cenaqlhu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3nqlbrmgs.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3odqjnury.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3cziidoka.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lawsgwre.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3seayznpe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ovvcamnx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dvsvwrip.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tlsmbjgq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3sjuaaboo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3igtpbnxi.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vsunfosr.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3awmfmodq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ffkhxtzu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3phhkgxbv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3glsapzin.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3edutgulu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3guseyvxv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3doigiemm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3pozqilgn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ljijdpdx.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3hkqwewlb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fmnbalsh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3oegrjwdc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jcdhfrni.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3tjvperda.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3bxlftrec.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rdzeevkl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xtgdahnl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hfknyvsu.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dqmiguyb.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3irausyzu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ipypdiwb.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wwxtazve.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mfmexdjg.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3vtnzfbpe.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nsalrodl.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dndvgwtw.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3vhkgbtoi.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3pieqbwkx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3egfuhalj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fcbupkmz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tfkscmjm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cvkklput.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hzkdrqiv.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ujnzwopw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3cjwdmzzk.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hnblngrw.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3mpyhwolf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3yzulsjry.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3lyndspgk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3mzeaismf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ezyjnuqc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zbxkagul.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3suwrtpgq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3iuqpuwzd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fnjrnbdo.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ededpuha.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gnszpgto.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3lbzvnpbj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3elwflcfg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3nvgvopsn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3pokigohw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3slbnktmb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3iaamlwmc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3xdvmqkqj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3bklwpoun.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3jrwcxzfl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jpopxxll.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3vbyywtgm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3dowmfjbn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3lcnprgco.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3uitphhtn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3qlvemttr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3vbzwflgd.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3mzxtthnh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3oheawjkc.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tapmwzno.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3bpdpvhvb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3vrbofatd.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dmdvrhel.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xmitrllr.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lvewfxjt.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ypmibcit.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ouskgqav.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hkyhkcpe.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lxlmxsty.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3unvwliln.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zliprcko.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3bfeqffqt.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dmjooriw.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3devoftkk.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3qwctcmfl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3bamjpndp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xutgwgkm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3vtvpaegr.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wacwlgdu.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lmkqvaxm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3fluhjwcr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3cvqgqgks.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3cxfnusuk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qsuhtxex.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3mqqfmbia.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ycvdargr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gcoqnrfp.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lbxhshxn.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cltawpup.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jevdnigc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3kpbpzbch.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3drzszrqb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hbfqlbno.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3qzbjhqkb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pqgdcmyl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jwvtjdwe.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3npkktflr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qvojzenu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3fqgrpges.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ofvbuxdt.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3fnobrpgz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3loizsfpl.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3nawoltgt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wmtnqruc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ezddmqqa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aazxuqkp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kcpbysxx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3yzdgtikb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3qrwojmxr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3suxswcwo.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3jyzjmtzq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ovbehzdu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3thviewrf.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3wpnyaljr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mjvkglcf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dfhtkbtn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3oxrbcpyd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bxffztha.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3xtayfcnn.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3iegtddmp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3tesnkbec.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3puffmabf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ynwkodcy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3egmnfbmc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3fuvuireb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3audtlfau.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3efnqywnx.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3hoxewmtv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ftjfuexk.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3xiqqgjbu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3thnmacqx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3saqsmpbz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3qgxkkzuv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3gxddmpdl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3gyperdhd.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3smqrnhfe.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3qknndstg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3vqryqfxl.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jbdezoxx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3xbouzhnl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rutilgcr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3wgxummvu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hrgrwkqf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3vinmaaua.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3vxhkixpi.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3fdaygjim.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3gevemmjp.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3cqqlpawm.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3feprvpni.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3dfbeeqcu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ykzboqau.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dhfqonaw.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rzrhpyqw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fkqgrsms.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pdmtbkze.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ensiphcr.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3iketrbup.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3txuzdljb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ifsaemjo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vrqlqdgm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3jaygjzgg.html


<!-- 参考信息 -->