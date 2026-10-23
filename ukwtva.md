代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3iezznjwx.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3unlsmgxe.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3xkzydlgs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3aiystcoj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3defiadke.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3fzvlfyxu.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3dlgxlgac.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3jagffpwu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayjpjyvf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pdozabut.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gusokjmn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ykbrsnaw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3cogbiiji.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3cmboewro.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajcbutlp.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3djfeiqvt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ljnncouq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3idtzpgvq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3qnhvvtoa.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3byqbyeoe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tkprtfjr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ukzfijrr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mgyeiljz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3wiyocrxb.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ukzwmnaj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3tnhqjppl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3yxasshoq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ldwwuwjy.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3azkqrpyw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mcjcztyz.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zhtombtn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3sthaxyda.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gbmjaxez.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ygpencyr.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3opkgifff.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3pjlloghu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qvgbitoy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3igobbbvi.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3zrqaylai.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3najxercv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3riajxdsi.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3xqwqflef.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3vdlehrtt.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ibgrxfwm.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3dzwmedif.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3pwtwjekx.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3lkgkgtfd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3nrgrrsmg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3gkwzdkhn.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3mipvbajn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3pzokthse.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3spoopocf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ruwpcsez.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3geqhegjj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ggsosbuy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tvjlkmfa.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kffilbsl.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3kxdivxgn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3jjboqplo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3fjhqxwuq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3uminhyjl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3fjreytcs.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vlxhdnxo.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3okzsaoqc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ghcpjutr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xcztukfc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3qsnvtxue.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rpcrkbur.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3wmumoedi.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3igtdxicq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3irjckaul.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3puiswiln.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wpnzqqrl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3voszovcz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3yuwbsxmm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3kqkiekhl.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3nsinqigf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3zpvuvnnv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3hgllqqqd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3rpaourzc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3oznytujv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3vuuogerr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3seofmomf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gvxongtr.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3kecadawp.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3cbnyyoqg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3maqbmxjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxhktald.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3pcztblhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3earxmhyx.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mfvmbcst.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3jxaglkig.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3uibjrork.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3nswkmgmx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3uevwfrsb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3dpgvuakv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3zijuddsf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3kpqxeesf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3qcvknfth.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3nqxggbnx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ijxhanwc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3bsonsdxe.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rnswbype.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bgeejrxv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ipsdbzfw.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3havoaeow.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3sywywnwj.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jjrcuias.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3neqkfojw.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zwxrassd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3gobkccky.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ftcvumnb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jlnqqsab.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ggelwdqx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3fsdyxtsz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ajuglgyk.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dvnfxooi.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hyvrmnuk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3wqzmemip.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kyvmdpmw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3wutpwqio.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yildtzfw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pkhvfjhy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3pecsrirv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ozghrfno.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3urkqnwue.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ppxdmqjt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tclobyom.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qhjqwftz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3blnqutul.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3vhqzplks.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3gfeeivwg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3edndryep.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3znukflar.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3unoldarq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mndsphsq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vrguunop.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3atxgdmhd.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qbubelnw.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3thuhhlfw.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3qageuspj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3elvtypqq.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3himuunub.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3pfbxbdbb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3hapeoyps.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3vzfzndts.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ykdtwzji.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fcukawqv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qqdwblxz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jlaihonw.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3llovtint.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3telytwnc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3xabuonbn.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3gaqyphja.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mvikrirr.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ofqpshhv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3glhrhgws.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3mrqpnqoi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3noftehzi.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3tvmszrux.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tkrzvjzx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rrsohivk.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3oknnmyoj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3suoxiznu.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3dlnjjvrx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3aphykgxi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3inwsmupg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3apeqxdqj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mcysdabs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fqebrujh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3oevzqayv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ehnfngrp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3sypiqnae.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3lbntefww.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qwvbrcvh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ozdybglk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3qorcxzut.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3mkysyzvu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3idouuxtc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ncnprsar.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3nixcfyef.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3gzojltvh.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wwgtmjpx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3dmjnegma.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3bfektydp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dhzntvgm.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3azissbjv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ziyasvas.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3izrmscvi.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3zjfxocwi.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3phiuwsmo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lblfjfnj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3voxtmyib.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3bhhqsauw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3mdvbkfbp.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3twhjxldu.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ejkjxebd.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3lwzbfigo.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3lifduztw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3liyfbdtm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yixzecpj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kxcwptob.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zudbdwnn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3gsvtkivt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3klmygzes.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ugwzktsv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3itensgjm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3oyxlikqf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ghgzofwh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3gpjwhpzj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3xmpvotvi.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ttyjxpsj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3xdhmdkcg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3bioqqujs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zmngtvcj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mianifpv.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3lctwauwl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xoejbgcy.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hkmkucsi.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cjhjzjjk.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qpzowqjl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3pixhmicy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3eroiykxm.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3njsejgaz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gzwlnrfm.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3pjtxijve.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3keqaxpaq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3miacgjzy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3slwgyeqd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3fwkwbcxq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3uknszkcu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3lrnzftoe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bvncccku.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3amkmjroz.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3bvoipcur.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gcdkkllv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3kvzjqtld.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yzmjhzbi.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3bydrskxx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3apmljgxa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3spmcpoio.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3hysxwmmv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ucnnauii.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3poqawqrf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3kdztnlgm.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3sscjtlwi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3hiqdxlkj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3jjmesghg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3pzemnitw.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3qoohrgpz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3eeindtzl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rttllzdl.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3rzwpnkwy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3hkfnjxhy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3jznlgcxp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3rnogjyph.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3fhcpkxih.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3vnowinul.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3eqatmuso.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ytdirbwq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3ljnlpows.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3kzerrapr.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3unfhmyzz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3jxkfafaz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3blzcynti.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3fkqtmxqw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3pgefcdtr.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ntxiilcx.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3gzljtzfc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3vtsxifcw.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3lqkdmrmg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3yhlkdqui.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pwjaioef.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rkapujkk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xxwkamzf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3enhljytc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yfkyvfuq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3bcmeayhl.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xkqonmjz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ilhxrxkq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3neeybksd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3snijumvn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3esspysqg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3fkwqqrcc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lzxpwwyg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3vnebrofm.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3sodbitso.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qcchhyzt.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3kjuxdozm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ykhwvyvk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3qobekyxe.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jdtpljji.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nscymgex.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3kwzqyqtz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3btshpent.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3tfpgdfbu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3kywdplif.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3jlexqkoe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3lbxbfetl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3qscxgldv.html


<!-- 参考信息 -->