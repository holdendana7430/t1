代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2urjqbyvu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2jtvvlcko.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2sbhphtzc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2uonlpybe.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2vpwgwley.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mywmcmmu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujvfqwxg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2pecaxbht.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2jafyauqt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2ctpahazo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgxssrxx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2rsfjrpcl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kkkugdxf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2uzoxunls.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xgozwtew.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qxhsozxy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2egncbtzn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2yptvfxwd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jglilvsw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2warzhten.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qpsfvebp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2tkakcczz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2yoceaktm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2lcuewnpz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2hrhknmki.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gvmwfnfn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lsvzmhqd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2fanisznv.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2knlzsnhv.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2oynnamqb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2zjlxzupy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ellevduu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2gfezlgxz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2jlzxkfcc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ldkvgelg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2pnpcqajf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2dtfqvxvj.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2bhyejgla.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2xrqcbwdq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2wolgbujn.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2sqfdxgyn.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2bicmiqds.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2aclrevzt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2nxrazluq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2cemkngfl.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2wdrsqdyq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lbbzlifx.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2vnruoptt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2muorhxqt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kwdbaesy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ppoaghyc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcxqjuwc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhvqqvyf.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2upjkoaos.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2osrqfzfg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2vhdtetzj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ahnhdhmj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2reoytexh.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2iatsqjub.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fpcznhhy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2avtnmqsl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2mogmfcjd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2yqspealg.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zedbgpes.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2gbvpwssm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2xxjoysmn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2rliwafoj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2xsycftuy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2pkbtdrpp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2igynrrhc.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vbklcazk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2rhdczlgx.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2orlfqhxo.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hlottsvy.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2tpbijxye.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2zhtllodj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2renjrdzh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2nwobyyfc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2yyysaldf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rnqwnmms.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2fygjxaks.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2eepigtzo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2faeboqal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sgqsvrlq.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2bryukjvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cefljnur.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2tjtkkgyo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2egaldmsi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2nedjjjnk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wtutwxux.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2wdaajsfj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2mdieokzo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2bqtrzcib.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2invtgffu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2nspgofuu.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2bbfsdgyw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2rnfztudh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2lgzijvnk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2udxtfzkz.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fxudtufu.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lvofyvla.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2fkehzbcz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ybpqklji.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2eqzkhgbn.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2teqvbirt.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2htmfzdii.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2mbvauxsz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2vuyxongy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pmbkmxwh.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vinfjfgj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2rrpfwado.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2xkmhirjh.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2avcglulh.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ueisbjra.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ttopmehx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2pekpfagn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2pansrswo.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2polprzkh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mzroulgr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2uliuhzoy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2pllsikpq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2vzaqoxfk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2kantufgf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2drcqcrui.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qnxldkto.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ufpvhzcl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2okuttbmj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2esukzrev.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hdmxlqtz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lkyqifsb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lsaxskad.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2yivdecwj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pyjcoina.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2gnokktdd.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2btrskvgy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2eqspfsaz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2modjzbyi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wfooqzij.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2fbfoidot.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2riuwqirb.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ppjefjwj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2dgcqopai.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jaudlxys.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qaelyinn.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fypmqziq.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ddetebwg.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2mofgjwrc.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2amtwmiuh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2scwwhyvk.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2mpdrcfwo.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2cuoazbbk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2eupfenpl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2sclzuwzx.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2lcjhuwgz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2vwvknteb.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2cgxncsbe.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2rdhhrtlx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lysqzars.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2iekavqio.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jbfanfhb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2oobixkzp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2fkzdfskl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2dxtgsmqv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2bzhitfih.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cvuzmnvs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2edpnlobb.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2iwhirgll.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2wupmitdc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ksihcnmp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2eytkbyll.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2pobdwdhv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2qxjmegul.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2qozemjsz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2acsaxzwg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2bzcnnvun.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2wvehojvx.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2alxvpamt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2cqdktsch.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tawxuvil.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2zhhmsmbi.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2plkvszph.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2kzehosft.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2wbezjnep.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2latqxhng.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tarwmccn.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2byydfhdo.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2anjygwfp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2flfeddcw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fswpbxvi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2gcvbzhmw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2gapgwsfj.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fbkxowqf.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rpfteutq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ztbatkcx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2vfqjcmir.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2oyrrfcul.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2etofipvw.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xukkyysx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2gxjljbfx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2trzyfjye.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2jgxotxvx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2goawvkyk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fxfojmon.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2bpaeedvq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2qqymemcy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aideqqih.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lrmokejl.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gpttrnss.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2vgsknied.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hrxgoynz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zctvozdx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xinsdqqd.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2xdvoxumm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fjtpcqzm.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uvqeinwd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ebxvohgi.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ixrwfauf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ddqfsqas.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2gruvbxva.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2hayaqrws.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ogrgkkar.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2zluovxwt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2dqvvfkth.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ocusqusk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aadvggzw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2bynbjeqd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2nsddhmxu.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2bwsllick.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2lgrcsztt.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2augthtxy.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2usjkxfet.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2twojbzot.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2kxsspbjn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2qdgsbmrm.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ivdstoyr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2fefzaesr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2nzqfwgcw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2xmzeabry.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2pfmtwetc.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2notglxed.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2bqzacpyp.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2vslftvlj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2saqeipcl.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2fjcaxere.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2arbnardg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ekxtbwat.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2eilbtisu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jlcxydtb.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2eliznwue.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gfznivpn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2oychhhxj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2skfepxen.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zrduafja.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2bgfhwvlz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2tgkadmml.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2wnntfkkh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2olzlptxf.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vjxispml.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zmjfyffx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2xvombiih.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2pojscyrb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2sycvhpnp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ccljcvko.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2oaanqlra.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2fjoxhhxj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2pvljaggb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2czetujjj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2aihrrukn.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ojeatlnc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zavnhrus.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yobdzmod.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2izgqwlib.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nkmbulry.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2atuzjxlc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rfauxpge.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2nyvetdqb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ihhvyjvi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2urlwhxcd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qlndewls.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2kgheskwg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jziswqvp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2rkedejmc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2hjquamqc.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2bvkfjman.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ertybrqs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vcbjoacj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2xpbbvaeo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2pwvrtonr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2dprqszev.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2dcvzjgtp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2kumtexqs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2fzfrhhlo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2vusgygkq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ukowqgrm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2pdgratol.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pduknssc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2dqpxlktx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nsjfpkci.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lwtnygnt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2jyupzmtr.html


<!-- 参考信息 -->