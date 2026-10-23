代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3obwozuiw.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3osvudmsg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3mwgojfnj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3tahbqyxf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3yxbmsydg.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ffbcxldt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3melcfmqf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3qmrkkxnr.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3igjdtzam.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3pdlzbnad.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3pfaccmbx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3bsrodmci.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3yykpptbj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3iznxzprp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ixskafyy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3cobgures.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3xvgsmfmp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3vzstymae.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ginvpgvf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3uzhoxfwq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3fdvcssdk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppmaroqt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3gkufpyjz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3dwgubyjj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3hsigdnsq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3qiiujftz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wphgycnt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3drnxovfq.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3zublllir.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3zrbrvglb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ytqogjxn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lygasuoe.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3nvpmgelf.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mjpvgvss.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lakatwrq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3oqpzqrri.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sevhzusr.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3zsgnltld.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3blnyfvni.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3mxajbmgn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ujxeikxa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3oitjhpoq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3fhkrpngm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3mojqyryf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3wvazisgp.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3zbunuvwa.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3mpemofqa.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3impkrxnv.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3rjllwbrb.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3eipohvkq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3lwdtvhwe.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3kwyifgrw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3zzqpqfij.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3svizlcyh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3crqtsbde.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3btadqddb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3auipzwso.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3foimwywl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3nzjodbim.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fngexzfk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zxvoheav.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3okyzdwrh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3xuocueey.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3treceezz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3cffsdubp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3repqhzyp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3kvjwxvds.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uxqddvus.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3gnlmwksg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibbpmywd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3uulsivzs.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mgzybffz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3qcqctjls.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3acjjtidc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3oxhpvhbh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ghbiwsth.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3vbkjknwx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yrrgxjbr.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3cclgebca.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3lxgztjcs.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3tnxotpdn.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3fusbcdlf.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ypvaqfrd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3yyxmsnhw.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ndxowmwx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ipxdwdje.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3znnngrtm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3erbbdauh.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3hrjrnmaw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3qmufxtae.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltjxqhga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gvtmblcv.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3dmytmzju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3novvvmpw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ggkszkpf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ykoxabfd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3sddcsgng.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3quoxeppx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3bqgmtliy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3swrxcuwi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3rogfqiwh.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3kkrylovn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3uixrvvyg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3fzbhguoo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ifpzyneo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3wemwvkgz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ltaikjqi.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qlnorsme.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3bsthgjqe.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dqfmtpjm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3czasmvvb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3hgxuytnm.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3uawddnty.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ovquidho.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3qhgdneca.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3bembrnrn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lndorpdm.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nmnwxfpq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3cierknlg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3tuvkxkqt.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xofdiigj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3wabhsmzc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sppxivry.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3zpqovlax.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3mhnlokol.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3zrblenba.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3yfbspwoa.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3sqohvjkn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vmywpeas.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3fvhethyb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3rbbfzqqv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jjuhxhwm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hkscpsjd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yzoisejv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3dguqgvtg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3jdybvkjo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rcakudjs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jtdegbbu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ntywoifi.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3eprcwqgd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gtowmrio.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jygcycxw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ywfucdww.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vugwybvk.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3jgwnrgur.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3arurxxrf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ygskdbsy.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3lhsvbdpw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3tnwrtkwc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3vcmuhtza.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3cwdxmwpa.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3eiwyhecm.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wkuzwdtu.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xkhgjwzu.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ivjbaycs.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3xtruloqq.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zdyyxniu.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3znoftumv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3irbiteic.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3qarbahbd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3qubdkckm.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3wyjvkebm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3coskdrme.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3lkycizyt.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rebgaxup.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3irnbtphp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3styyqqov.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3whzymkfl.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ttmkokzo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3hvkwoddq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3slfqskxm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3wbpswqxl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ucrmtxhi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pgxerhee.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3lwryyefr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ehosqjfk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nmgurjfw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mvzfstpv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qdqqvlbd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tezpteiw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3mhfqaxsb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3fbgtkvpu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3vndwvuhj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3azjeibex.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3xlqonbss.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3iulzgrjo.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3egwvwcjx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3uvokdsle.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3cifzdujr.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3putyrzxu.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zqixfnhh.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qamilxot.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3gclbgljd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3sprbzoff.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dpfxtwyx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ldaxysqe.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3mtvcmvfh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ojutgpwb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ngvwhoes.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nuzcfxfs.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3lbwdjsvb.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3yaledzaw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3vbzwnbxp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3injbdjda.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kusqwmsc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vfflzref.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3khmtdtuu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ppkgpyqg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3xvyopzzc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3fbcbxluc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vuitzfac.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3zgeersmh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3jbscmplq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sfeuoyqb.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rlotbkqa.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3myljwnos.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3loabfuvm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ragdzuao.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wlpooypo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zgvjchxn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3zvyfwxlj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xeulgeqh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oqzwjnzy.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rlbivklc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3efxvgvzm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3wfmixhpe.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3puujgcen.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3tkzxbxfb.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3myrzfcvs.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3lfvzlnxi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pkfavmrw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ucsoeymo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3epekcyfk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wrwtzprz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3dnnhbmvi.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3yonlwfqu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3rxralerv.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3jscymadi.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3cjvbnlan.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3pcdsgeic.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xqiifikf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3cxocisgk.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cvmiifpj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rfxdpkck.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qachqrfh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3vymrbqie.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ujbdhycn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3dpnmzfti.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3fxinhfqq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3tfwoodrm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3egftierr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3nkjiqphl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ptbzccii.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vqmwuhvy.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3xgshfydd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jlfhkfrx.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3pukoupqn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3fjdnmijg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3agkjnorg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3akbgfjkk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3kkcvpxmq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3iphtyniz.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3lwswkole.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3uxtutwrs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ueiosisq.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3udlgwngx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3jcahodbr.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3yckmcwph.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3pxebqepd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3cviedpqe.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3fsunffah.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3basbyycx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3uqbuwkxq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3beolepgp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3nviodxfr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3iwgzyjtn.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3hwjkkmfi.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yjlznzrd.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dsehtafg.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gtuajeok.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3obxlxmrw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3xgatkcit.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ifigkrhq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ozjvwweb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3igedmrxk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3hyxcwnbp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jgkywzhg.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3bbtsncvh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kvddnvdv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ktsmfunk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3pwhwhtue.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3nvyigazt.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3cgqfbdyq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dnfzybcm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dalicapd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uumzlguq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qkgcgtbq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3hizxlukp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3etehpcvq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3paiucryl.html


<!-- 参考信息 -->