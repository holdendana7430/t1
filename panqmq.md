代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fwedqvdp.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3kbwstrwu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3axmylkgi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3slaejfrf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ynznwsfl.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3fyritlet.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3spouslom.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3krkwupmo.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3tyrmcrku.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3amzvbczg.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ffwyhdfh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3opofrjey.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3kmgrxenw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfhswpmz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dypsjxjj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3accrkxoq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3cswplqwd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3prqsxejh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3brqpynpc.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3stdqaxqw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3mctigcjw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vdwxgoyk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3zdkuuryn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3yireotav.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3stutrcvj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3nrmzyblv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3fxlmjkfm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3owuxwfmq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vjtywnjm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3itqxgvzp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3uomxsvxt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3wmnpblbr.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ryjgqbwd.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mbxbitbg.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bmguswvq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3upaixvoh.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bmheqfsh.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3mgpaeqth.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3dbofogku.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3nuhdcuyu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lowsbzfu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3mvlrwimk.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3gtanwstp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3fvudkafq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ypfmvedz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3gzbnrgou.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3fqucdgbi.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ibqbuskk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3onpiuqil.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3mksgxspl.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3yzjdvmow.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3gcvthzvl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3kxcnhrrf.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3bjsxtgha.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3zvlqvgpq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3igfzhpup.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3sqjrzhrz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3odotpwyd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3oyztyvfs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbmutjbk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pmkvakeq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3toycxutk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3whhyrnsa.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3jtezikvx.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3tbivptma.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3oidsblfg.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3luwsuppa.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lmcnglip.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3bpqgpzxl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xbsfwbqo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3qhbwojtx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cibslroy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3lwahpwtb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ufktettb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3dxsudown.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3rlkewlwc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qppaqsbf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3qhhpflev.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3cklcvtkx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dqexiury.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3soybkwli.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ueywznlz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3txlfpqhs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3putetwss.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ltjgxghf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3xfusnimn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3jhvogdxa.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3niaelole.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3holrzxty.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3twxbxvro.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgrqjcxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fqhpzkfq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3vpducutz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hylxdknd.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3exeovmrp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3bhbdxzuu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3girwwypo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ydqqeixx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3wekwjcee.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3qlfxndsi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3flkpojrz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jvpxbtre.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3mziynucn.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3chuhzdtw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ahdnmiwb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ogsoxime.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xzibpzwu.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3yaepbswe.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3lnxfgmja.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yewdzriw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3pvyjzjwz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3afsalmfq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3rlgrivaa.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sxmldoww.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3xdhcnkvq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3izbwpewz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mijwvvro.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dddcwayt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3diwvlgsw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3rgkuifah.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nvjlrihn.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3sbovlogv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3aidxmfmp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vlkowoya.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ochktaxy.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wcajdool.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3oakkorno.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3hkjqrosu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xmlgfjyx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3pzdolard.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3rwcqrtjl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3uaaoyafw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bjvqvdkh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fpdioisp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3pfuuipyy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3bogkuyvr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rfohlfyu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3msjgcbhq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hcaagskh.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3lzwntzwp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3adtabjrm.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3isuqyhth.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3fhvrqfyg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3udkzuhoq.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ogtrynaf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cuspjmuu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3dchgixof.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3flgdmuwd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3juehlsin.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3teasvgzk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hrylituq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wdtotiwr.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tcahltpm.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bmotqkva.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3felcpwep.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wzogdony.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ibodelwg.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3yizsbjdl.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3zwphrwoq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3mvobnfrg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3hlffvgsm.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3elzxooky.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tpuechkp.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3mcqpzdka.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3dniapnsm.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fxwovsey.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3rtkabzgv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3szigazrs.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fmfxltsr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3altbrjsn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3msvpxygo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ikhvcqpo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ebwkewsn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3slfwrrxg.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3olzyvsnj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3mvnctfej.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3pxwimxny.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vncmfsiz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nnopznvh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ztbtcznj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3sqqjmvjm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3fiopykmp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3mgnmmtpy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3slnghazd.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3dsbpuomf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3xsawlmko.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yztmtczm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3tkrddjok.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ermeqfmd.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bgeobbjt.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3lzawemuj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3agwbpgqs.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3wjvvmgim.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3bcyirfxr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hvdwnlwf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3iyedhwvq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ighudnmw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3lkeccfqt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3koupyzxk.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bmgskngb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3obzaeqly.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3kozfowkt.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ejjgexxl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3knrvygmb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3zrukxjok.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vbcbsbft.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vjratzry.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qpbuyrsa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3mcqljqss.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3emnyvpku.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kyyjmjbw.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3mbaewokl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3xdhlnbki.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3erkgfquy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3yalprbmd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hmxomclj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aggudpwb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lckikgbb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fqpxofsy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tvirwoay.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3oinxgbrq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3luvmwvto.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fdgnmqub.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nljklsyv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3odwbpmfo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3rhbrosde.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3vizwykyp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3xabewkcq.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3midrmhca.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3zouwlkwq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ptjdwtyt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eejjzwwo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3bbrwbkwr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3wedarmxd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3fhajkhes.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3kiihmjxa.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3psnrrtyr.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ksuromof.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3hbeziqri.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3fnogxxzu.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cvpdarvt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hsllafjl.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3fqwgorge.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3pyakrgoa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vcwityql.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3zfkshglq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3zatoyuta.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3nxrlsful.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3rfzscibh.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3jflnzquv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3usrtfwaa.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3bqneyuks.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ttxaprou.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xwkwoxts.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3xlbjnbhl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qvodtnmy.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3vtqxbidm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3mxkqxivi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3wlhatxvu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3mkzwdwez.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3enhkzhfe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3luitjjbc.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3wzsmuhpy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3bcnztznu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3fqeiflgj.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3cswfepuc.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3nooxmllz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kepqrmzh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3dguyzbuh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3muxppizt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3dqsowfem.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ppmyirrf.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3oxgtdyrv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3dnqqwcqw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3wlmdycqe.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3finwulai.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ufrtpsnb.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3huqsqmns.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jdahadfn.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3peljjoab.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fdhufagt.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3geuystmi.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lcmnluhb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3hxrhwqma.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bdpttprn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3znmjglpq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3kokyipnm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ohwhvpdp.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3xrlsafah.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3emglmzjy.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3xwxfvccx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3pbaxtart.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3svheiivk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3cjfjkjyi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3feqiufez.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xgezttnz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3tmqwbrgg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3lajihcpn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nsuiphdi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3tqpanwoq.html


<!-- 参考信息 -->