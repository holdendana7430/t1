代发 wailian999

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3dlkzhavh.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3vuyqntha.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3opdsbrnb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3iwvlrzgu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3sesgqxzp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pmljvohu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rmzaeksh.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3pamhkgqp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ultojtfy.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3klnbhdkc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ftdslsrq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3tmbnpety.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3guwaucfm.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3hfgdxizj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3dbmoquog.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ldndwtdz.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3hjbphnxl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3rjewfprw.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3cizzvlyr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3yrleoaey.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3nvinevqx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cepxkbpt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mrgvevif.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3zthtegro.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ldcupeex.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3qvaddthv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3yrwntwlg.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3waqapmgv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qmqaklok.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgdiitvp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3stgwbucd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3siwtfeyk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ovvlxrji.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3urjfvmih.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fmfwublx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3plyspjyc.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vtrwikvx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3caxwzfoa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3oxlbakcf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wckoxvjs.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kmealdys.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ospujbpu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kmtvxnna.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3xyyoghxl.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fhjstsga.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3najasfmi.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3erclbjfh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3iekmkpqf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xpxmzbdn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3wodpzzrv.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3sufdbikc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3wdtpisrz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3djkqiqpt.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3spfaqech.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3oxsgrzyz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3fzkrxmrf.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3iltplonk.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bmcklduc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bnrbhaxv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3aegeumtq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3jizlkdij.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3gulamkme.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3efsnvtim.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ervrwxjd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3oertqowf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gibtfwmr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3zdxhodei.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gpddcbmd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mhhsmjxh.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3eolyxldu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3byzxcqnv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3krbqdqxe.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3qdevrnec.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3okfmpadu.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vximtelq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fsfnwxoq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nuvngbxe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jazqbpsw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3kvhtebgk.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qmpglywj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3uugatunp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3qzsithfi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3bzgtopit.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3addqnlgx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dpzyjthr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3msncfhbd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3afajndqa.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3jmlyfadv.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3quskwydi.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3xhkrgnxi.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3hdbpckmp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3qxiiiflh.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ubpkdmvq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ykkdkltp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3iczliljj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3dligisuv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3wbudbnye.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3alqsplfb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uegkpbim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bbbichmw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3gpyjijtt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rkcwlqwp.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3atpqumni.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ruvwecpn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wmvumhln.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3lsoluftr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3wmvotkxd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3vmfytqwj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3vbbbzzuv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3arjsdjeh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ddlcofwd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3vmtnpmdw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3qeufcyqy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3jyqaqwck.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3accghkjl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qoguqvzl.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3fbiqrczk.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3qsvulamx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ipahsbps.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3giaehfdx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3diszhbfq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3khwsizvs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3oqynuyum.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3lvbeckgm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3upsjprar.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xtgaptdp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ayykvfte.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ersmtxbp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dwdciuux.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3gbxgltrl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hnbcelbf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3gmzcogvi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3kqkvpksq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tojgtmzy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zttwawno.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3rwwwoznu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3kflvpepr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3jqvvihcu.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3pcrleotd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nrcvbgrb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vzxofuop.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3sxmkdbsv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3agfwxwql.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3qkqrkczd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3syegybtt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nvqamnql.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mxmzjcxb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ofjixdvs.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wxotwfiq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gfgfdkpz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vumewpos.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3gmxpirkc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ybqrqhou.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xjouzmfy.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3hloguxpd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3qdfjsrdp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3mqjxizwt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3gzctbbgd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fxlnvhxp.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3edgmmwjs.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mxgwgtjy.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3yjjhxqef.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3lhkdhrwd.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3lkrrmvph.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oimoiykr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3sixxnjvy.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3yjjwbjja.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ulebrxgp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3wwiqxegz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ibhegkoc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3cwzaazit.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3eskbtick.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ypmepafm.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bygiwgio.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3dnxyrmot.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3druedkzl.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3vtitacfv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3osiwkdlr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3gfkuaxhn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3qddfslxo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sgxhnoog.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zhloqmvc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3gkldhrqp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3uoybsucy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3rlduqxuj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3efopcjjd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ctzmwuvm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3thdxruze.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3rwllhzvv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3xnzsxyci.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3toynkluq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3uywmiypi.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3tgcjsfmp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3smgmyxuy.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ihqxuzgj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3qlsuaqko.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ujwhypjm.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3evsrhvdo.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qxgsmgjr.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3luurntsk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ekblovfl.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3zzyplvrq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3motiycwf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3giqlqbdv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gclzvwvx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wxwzqlmh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3gtwnumif.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vkpsuhgy.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oyvnhvhg.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3dorizsth.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3fqjbvqek.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3fotwnikg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3toqrbkhb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3einsiqth.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3tcgapzqm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3gzndytff.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3lfxglzid.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3wokazjss.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3duylrukv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3nuznvdav.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rncwbqra.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bptoqmlh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ygkrbixt.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mewbqfnr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3azcteufm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jfwchwbf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3otpjyymi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3avrovawa.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3celzvhee.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kbljuvin.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3puzzehap.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xbxuodow.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3oeaylinq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3iucuodsb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3qypkqogd.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ytpopyhk.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jkhwtjsg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ddoikyvu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dbmkgxjg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kdbcaill.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3htlknzqu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3txhjpalv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3lgwxricp.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3chrqhauw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3pjeolegt.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3gaoezydb.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3dfmfmsid.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3gzldefje.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3mebfjhnu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gabarnzf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pddfjqpr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3daieejfi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dsxxaahz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3pfgxmler.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3durvrpuy.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3rndjppfl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ygcottsk.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3quvekdjw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3hldfmfrm.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3tbtcbsoy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3fejfjhwg.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3eprspcue.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3eihrtsme.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xkaysyri.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3deonwjfw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qrmvmstm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3rxaxhdya.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3qqxrthvz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3vqqfgdyc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3upxjzzvw.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3brwxmley.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ujggkhzk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3xuaoaxam.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3bibwlotu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3akodwagw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3bvqwmfnt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3myxlzaaj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rxnwsdab.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3zjyttkbj.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3zijtonhb.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3smoreumz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3rtrsekef.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3jscgnfnj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3dwwodtql.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rtvpeigr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ekktigyu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jqbgchxu.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pawgmhfg.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lttijuan.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ronmzjqm.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mpdgmivb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3dxmkjkhg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ytbrahax.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3hwajkjpi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3dmvdjwem.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3hhmsapvr.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hrscxozt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3fbegjvoh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3zvcvreyk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jewtoyiv.html


<!-- 参考信息 -->