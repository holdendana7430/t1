代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rymooapc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dlkazgjr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3acqdupvx.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xjzzofze.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3iuolocdp.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3wcvfnlfz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ikpeffxq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bzxxubkb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3gtcwocko.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3yfbhpbjm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ogcvqxjx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3xzmvxrcy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3uirgppvp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3buvcovkk.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3lqetakjv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ljtclbsp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzvzycup.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3egqldhxy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kohisnis.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3dfxqqpgh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3nyrehprr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3widqxhli.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbnjehfy.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3lpntsxze.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3kvsocxvv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3sculrpqx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3uwvxdabh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3huulkola.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3vzwluxzp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3xgvdaede.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xlozmyek.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3evildidc.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uoihgzgu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3oxqmbquc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3lsdpcmzo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rqybcvng.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3dygyvrhn.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rwusubaj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vdijeaxy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3tfjhcqjh.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sjzfjniw.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3bbgjmflm.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3qpywxvmd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3fsssqqbh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3bujdoitt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3wanzsbui.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3spnomchc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3nuwkekqi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3bwqlgshs.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ipxbeqbe.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3mivgoziw.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3bolavpfc.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ouxqrgad.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jccqxeqn.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3gonbejvp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3gwnstdeo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3pwawfrlf.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3zgycnoee.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ctlqbvhb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3xeowrkxz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gxgywpqt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvphbzlt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3zxmyeeyo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zizntaha.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mudtmihk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3wuyvssos.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3yivkzcdj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3nwiubaai.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3zmirjzpj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3twvbxsvl.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3kfshyayu.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wmlmgbld.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3wxvdgsvl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vcywxcdi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3mjouwwjb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3oydvvvan.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3jtbpafqr.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ngmrkyxe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3bvbvjitx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3yotwqkqb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cyledbwq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hhcvlift.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vrazkqlj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ctdpxjmt.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3wxieezrc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3erzjflpv.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3feuvzvtk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3abgterhx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3pwxandbn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3aypbgowt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3gtcdpdkk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bruptjpi.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3venujjjz.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3wnbicqhh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3rvuneiog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxkvonar.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3nvffomsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nzknvckh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3kyytxizt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3gtufqoub.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hfjmsldc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3gyyhqxge.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3uoqvript.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3thzzqbxo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3xbuvjpom.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ifpcttkk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3nvgnltbx.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3lnugvivf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3smdzbtrz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3qzqxhrdy.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3kqlxadoz.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dxrqcxyb.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3emylmmxt.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ccvchvte.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3nzyxsqjq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3odsheplm.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3rzagrvnd.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3bbsrpdxe.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ciqrbsjv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3pjldlmfu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3oydhvssf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3edjwgscx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hmvtprif.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3sydsgqzk.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nfzmetaz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3dmtouliz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3nhlwlysy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3varowodw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3vdpixnus.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tzwlghle.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3cmymkafq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ljqyqzmh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3zmnkyytg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3movtquaq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3xamijuqo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3quphqckq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3epcnroop.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kfzoubna.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3yozvgevz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3pxwlwmqi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3pajhdtcc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hoswkghz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ymlzxhhg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3glcvxxtn.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xfqzcnfk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bupqytay.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3uozujnyn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qzenible.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3dtzxoaqq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dldjmhud.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ilvibnca.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ugdlnusy.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3eyapxrxf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3kivptfwh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jempvxtj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wnmqdvvi.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ghmwwmqs.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3trmvdhmp.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3pipxmhqy.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3knoqsyrj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lciazrcp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3zpfwdfns.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3xjddsens.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3sfzjvbgp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3rndzyokc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3gwnmhhfb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ykfijmyn.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3uqcyqayz.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3swysgaqz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3amrjmlnr.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3duxvznas.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3aquafohw.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3arxqsxfv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3emunjecl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3vwhewqib.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3laqlwthh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ukhklawp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3yfgvwtzt.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3afatiujw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3rpbsctzq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3uxtivmcn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3erpyihye.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3rkgmhmfh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lalraaim.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3tbdmuosd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3dsdvfmka.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3zecvgyxh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3azivmyat.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3phfppvdd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3epbivqjk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3gxxdcnvi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3mwmlcjuo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fnybaubi.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3uxckxshz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rnvphtjw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3nepzzobn.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3akqtamrb.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3kluhshwo.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3cifpkavt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3nwaxqcda.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kzrpsurr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3btecgtti.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3zaucxijy.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tfcehsmj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3bfvsnhlr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3jgnrsgub.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ffzfvcfl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xzmsxaxo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3szexwpox.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ejifqsvy.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tziswode.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tmihyxcy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3jaolgagd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3kpuysmqe.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ljlssolr.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3usqypmue.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ogrotbpr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3prtxbmxz.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3etpcfkpj.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ftzprggv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3kjabonnm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tnsgdmqa.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qpqnkoig.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hehhhrtz.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3nosnacot.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3roohcsyy.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iozgysbz.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nznhsdhr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jqgbphos.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3xpifvgba.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3cbewdhqs.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3zijfwxar.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ndxcfzdy.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3xeggynmm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qxyhotbm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qcoecizt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qzagkdjv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3tdxrcppa.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ynnfhvix.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3maoknmtq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qkounvtj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3mjljrlzy.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3etovxlkv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ibwilpip.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tibishif.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wvsouifj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3flzaglov.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3sfjgmstp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3luprljmy.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3kqsvqtrr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3aayqeyeq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3rqbomqsh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3nsgobogy.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3vfyusuey.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3palkrubo.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ewktipul.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3yjpdkmbl.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3utatejpc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3xdehvfxu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tguevnux.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3vxomfnjr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3xjdduicz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3dtieuzzr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3qemvjvcq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3bqqdgmme.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ybvkhkpy.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3mbvavjoy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3aumbwapn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3uqnztdrt.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3eybcekpm.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fuvfnava.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3yrtwmkun.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3dbjwxhfb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xugzqksj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3lcsrxxks.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3efrawyaa.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3tecmyher.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3comdessl.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3suxkgeil.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3miaitjfi.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gfuursue.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3siutenje.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ufgcbvyp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ladipwhm.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vfbwntji.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qdwtvfbx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3efbjvftu.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3rvsrbpdm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3owgcfkpq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3nqhdizld.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uwttywor.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3pjzpzoyx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3gbxoosxk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3jkgueaoa.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3jftffsww.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3czwrpymf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3typldqjb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3weyatisv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3nyrttzac.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3txbitwit.html


<!-- 参考信息 -->