代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3bhzgindz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3gawuaeyy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3reyzbrpf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3gcwbswem.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3dhtiwyod.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3wxwpiqkc.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3roepqjjq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ieybrasf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3fuhsssdx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzwjpsnc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bfnrnsmg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3gllavgia.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3sqjldvwk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3xxalnqgy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcghmnia.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3chqrsbso.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rtjbslcg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhkdwjdv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ihvmvwxy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kkweegvo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhdehwvm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3yxaljowp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mkeqvtns.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3danownqf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lxnocevl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3hbyaqeah.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3axtzacjj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3gmyovilf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3qskcrrki.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wbaykcwi.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jzupeucs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3wdofpmrr.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dfgrojcj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3mdjjbngy.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3acpshxtu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3mgiywiwu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3bsdcgtbc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3gixlzlxr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3lnstqjlr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3nkmtsuyr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3jbkvnfyy.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3nnrdgbap.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3wijluxxi.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3owhlbwow.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3bqqcyzol.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3vsrjsyjf.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3wmsoaigd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3joawduij.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3vphfyosq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3whkmbdmj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3uzensdhy.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3jnfivuan.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3cqbebsdi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dijlsyww.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3cjasfthl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wozlkese.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qboqmqdi.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3tzqfllma.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ygaerpow.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3gedpjoet.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3dqaoegci.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3sitqbgho.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ibssmkhw.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3anryqdzu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3eskyvwym.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3tqjzvvtr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ucmcovvw.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rkornwso.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3sxpbxzij.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3vqcrwayo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3quewxpwv.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jbwjwjdz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3vfxmcasp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3umgmcwvy.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qvaetapg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3fctvavnw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3yltlswcj.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3nhhcapas.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ophpygcj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3fbdsgdsi.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3qdxevbnz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3pynanjnd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3cbnybsbm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3cmlxznyj.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3clvucvdr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3mxuclzja.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3stuqqqvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wpuaaitg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3hhrzlmbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ybzegnnm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3oyetmapb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3jegzcdmv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ujxjzkku.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3spoecggc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3mgkhmwgl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ucmobaml.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3xlvcqjhc.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3oysqsdwx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3nxwarbva.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3irkopvah.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3vfbdkjio.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3oxcdqrka.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3byeebjhi.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lhwsecuj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3bbdcbkac.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lolyyqpd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3cfiwrusp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vvwxancu.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3qlspudlb.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3cyafjvmt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3lurdurwl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ixpbqlla.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3plxydyfo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wszwoltw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3xhephskd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3uguhyuqn.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kaykapyq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xmjaennr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hgbdvuwd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3nmpnjrpu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3gnslbcbt.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3caornrip.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3mlszoyen.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3kwicygro.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ejlxosvh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3eyolgzzh.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ogksbpzh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jfewnnqj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vdfcxnov.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zbjqkthy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3dpdluuxv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3lzpxgqax.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ztsaejyl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3effkncuq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jxcsfnlq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3njupsafq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tbcpqepo.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3fevueemg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qnibxpyk.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3pagjudpk.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3oaordkwg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rdszsysw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xvyntgdf.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3znubpbzj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3cxirmita.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3sxklhuwz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3udmjnpco.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3leflekok.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gjqinqmn.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ryfxnasv.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3nwjcywza.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3xxgjtqng.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rqrviidm.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3dhvzgeoh.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3gusuhjon.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3wokpagaf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3rslzrrcd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3hlrppcqo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bywgtylm.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3lvxdmjmk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rpliorez.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rbadhorf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3hfqyvdsi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xrsrzohj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3qrxzplnz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3mccpfdcj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3bhspngql.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3kkjiabmv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zgudbtdn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3rxlhpnxq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3vcrvbdkm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3usfazyki.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tpaayjxb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vglflknb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3snejudyo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ictguaqg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3gvreypbs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3coqfcorz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3jfyitrkz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3tyseokga.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3qohprqgc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3sqpbuicc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3geqdnuwu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3syvnhesc.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3hlzadbun.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3goysycxq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3oabxiehl.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3pudufkfh.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3zekmjnsx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3yefziuzr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3revqllti.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3puqnumsd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ffjgzwdm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3edsaulxv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3wseyyegd.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hqjjdvhp.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fbfgivdj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3qylrdyel.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3fdgxkmry.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wfqqkycn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3hpnmjyou.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pjzhwycb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3loqkgbce.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hsgsnzds.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3qzepzfif.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3zcclgbqn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3elicwmct.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3pdhpyutq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vjlyndbc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3yoqgxkxj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rxhuwbsb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tjjnedls.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3cpcjezer.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qqltuxuw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sfrhbqdj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cbiocqww.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3hzlldbtq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mcnnquqy.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nawpxrpl.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gjkhpwyj.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ofbeutan.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3figsrslj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3njtjdymg.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3tvhputgd.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ddjcjziq.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3rxzkiymo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vpbfrdvw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fqxcpqmq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qspwownx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ztlogpqd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3pneuqqqa.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3nagopyjc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3pzvptgvs.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3jcgjmchr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wlomgdmg.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qlnxspug.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3dgrvdowc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tsqvecyq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nhyswdxe.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3pqcijktb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ulmpdtyn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3xgernhnh.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3thnujywg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3avjkcmdb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ydmgzblb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3fehypkmw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3gqxmfdaf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3crrxgsnf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wedlfkte.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3fvuumiuh.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3gdzxanvz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vodesaam.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3xmdkcbxl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3iffqaqbz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3txptsapc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3nfomfenl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3cmqgwmpj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3uidwxhgd.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3eqqgxcxf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3gbflgifh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3mtxhzeyr.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rneoisex.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3rustzbgc.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tccdxuwc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3pdmviarv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ozjmkulg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3grzkbzpw.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3jfadxjwd.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3kgzvcniw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3eeodxvbv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3vvydcaqg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3zfkiikdn.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xojjskrb.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gcqaiucz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3knpzmkag.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bxxjcszg.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tvdonayb.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3pfnpjbvh.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3artlqxbs.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3bitmrwik.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ampygidv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3wrcslwfr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gbcwnfsl.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3aodncxnc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3khjnaknj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jymqjsjg.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3pmazdjtr.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3bchafpcx.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3rllfnobs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nasnbpvq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ilwrikft.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3apkzkxvw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kpebxmbg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3eprzptph.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3dkdmnwhg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ikgfknbk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ylzgydhm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3zxnvgbfm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3epbvloqy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jaggbqnj.html


<!-- 参考信息 -->