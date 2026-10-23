代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wlfwinxf.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3mpqfjalu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3juuqlbww.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3giihdfym.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3wifzucfw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3gehjfnkx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bvzykuij.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3gtzhcjyc.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3yqdptiox.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3rdqsmjkq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3kpqeiunk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3uqylmufs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnettsew.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rwqvjalx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wtjwhkvl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3uyrtfkkf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3xlaeledg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3uojnbioa.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vfndatdr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3rjoufdqx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3udrnmjqv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bxvzpocg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3anuzhnkh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3hbmxunqd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rtelbeuh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3eytjehzk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3mljsoixq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3mgmwhceb.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bixaozzs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3xpziayer.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3wmkbgvyg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3etjymcdb.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3xpcuwdlc.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3etkxosap.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vhxtiljz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3yqwndzyv.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3frgyynui.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3nxiolvpi.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3mdyqmtea.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3tdaxvddo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3djivesbp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3hlfzvqmi.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3paezzaga.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3qgbohhqt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ojdsvmuz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3vrbjvuyp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3qtplsldd.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3dblaufqt.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3nrqrljby.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bzojwzmo.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3gpungdon.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3plrtwrzq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ypvwpmsy.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3btdfihbn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3zwnjoigy.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3yvbhvdrn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hmnpjfyd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wgjyqwty.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3mhvuiaqm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3brwcwqji.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ohixqpzt.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3oogkjwlu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3daguxqho.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ykvnflcu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3jyiukuli.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3bnmogwwt.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wifshowt.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3slfbxwdm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3gmtaxiii.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3qssrjzic.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ffsnvhgh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vgmpjzue.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ixugqnjm.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3wjksrkhc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3slikusmw.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3eeunduyx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3klawqtbh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3niuvheoz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3egumbdqo.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3egetzayl.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3hqgnmuis.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3kdurdaeu.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3qoltzkzx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3bqnvwiit.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3smviewuh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3irzghkuw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3jcpulbjf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ynlzejoy.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3cctwydts.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3pmxitdde.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3tomugovc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tymtmrze.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3wtpoctdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dxwfkbpa.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3izxuqsqv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3hjlsqadj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3rnomayxk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3nbjbdcep.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3rnhygavo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3puniqypn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ofyonwbo.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3avjdvfpw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3vmpareka.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3rkmhnpdz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3feutpras.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3eezpwbbd.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3jjkpdien.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rthdbzcc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3vzmcrrxh.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vfcumsiy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ugpherxl.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jcojvgsu.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3nqfciwrg.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3werqasbu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3qeueghpv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3opagxcqg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3iilqpysp.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zsmwsars.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3lclifhom.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3jtuwupxg.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3unkcplym.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3auivjrtu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3dbcvkvno.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wxduqxsz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3fanyrapx.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kggmslpw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3tbshewfz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3eljgcdpk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ysbzsacg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3dgrenqvz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3fajuuqzs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bnlfkfrb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jztqoevy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3oahtyqyy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3wvqeqkzu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3gurxtlll.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kifwhnll.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3smohbtav.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qpyupmeg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3uxquufyc.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xriypyai.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kgnjzkct.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3gblqntki.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3tbeyeopy.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ugpvaadp.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cinamloh.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zremnedj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3xenldege.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ipdjodmk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3gpkxykba.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qfapjdcb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dbykmqqu.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tsrccpze.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lklnmqpc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3nwpejgbz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3sztgojwy.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qfqfmseo.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3zqvmetpr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3hyepvlcb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3zuaaszek.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3neavxsyf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3kfgxylaq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yboqqwtf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3lhnxtozu.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3auxdcvln.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3afiephsd.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3fykvcajc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3bushfvlv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3thqgkfnd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ilcsqopk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3tbdberoo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3mgdqkcnq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mqtwmjfx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lvuflslr.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3jhaehtne.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3otkccqcw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3komdquak.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3exavqbyn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3qjazfawa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xjmjntkp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3weacinfb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3gfrkmbcx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3xyrdfbwk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ilcgqknd.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3asbwbrsh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3rvrsjclo.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vgslpayv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3jehwokes.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3tavlxjmt.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ivhyxign.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ihfnrcad.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ywyvetwx.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ybvwfiut.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3jptbuedw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3raiewruh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cwfkaowz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3xyzpfpdy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ctiwhdsy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3rrqqvipj.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lydgngji.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ykctnraf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3wbyzzeef.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3kbijacei.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bbbfqpgn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wbstwkgm.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3kumszojh.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3urazjisy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bwszktpo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3cfqpdrhj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3xewborqh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fxyfndtp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3tqksgkcv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cniwhoaf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ynushqfv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mpgyluob.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cuksipdx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xhgcqvra.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3unmqafgn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jhoctvmr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hbsrssco.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3sqmtuvhi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zwofvxor.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3izahvupy.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ninsggkb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vgawgfyx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3obvgtrxd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3vjtupzpe.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3otfpfzjx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xnmiiseh.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3uzqrcwtw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ovmjbzbd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gjagqqpx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gadapqsg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tghasojq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3qjrmmvlk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3cxzdfxsr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3htbhjkcp.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3mdmeofni.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gbclpgtz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3pmnmqqkb.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cacqklzq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wqcsvfqv.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wyzokrjp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3bhunmhaa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3exavqebq.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3sjzcvrkf.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3epxlbccz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3hwxrofay.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3tsuaonop.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3xgwjlyjd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3dmrraqah.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3atzrwwwl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3piuivmdg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3yiiuezym.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3kuvvrlfj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xzjabdlz.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3bvcgqtnc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3zkgzwjoj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3pplkjeii.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3gdikdzdu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qwmshpcm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3thxjdpnt.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3nkpxafam.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3syuncatg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3fehqwjdb.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3paymqbtx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zuiiochu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lblphsld.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3gjnjgzla.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ezgxgypw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3lsmpdiao.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3endvzcua.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3rqnnifqr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3xypvudbd.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3pfbhmwch.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qvaxoobi.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lonhvrfc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3itxbaplc.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mscdquuz.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3osmdktda.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3svgjgdez.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3uevyrigk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ffxidsxi.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3qfmnjavs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3bgjemkqa.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3pwvjdqfw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ywhfiald.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3bkjoepjk.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3xrhgggmx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hidrazfq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3lfoieqzs.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jjjpzvzb.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3zkqilxyb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3tofgmnnn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3stglfbyt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eohdxgzb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xsnygzpo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ohuwgwos.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3dcwxjudz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3kocmihvi.html


<!-- 参考信息 -->