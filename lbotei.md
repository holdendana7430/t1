代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3atyiayvf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3rnynojxe.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3eaauicjm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rfjsiyhy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3nkeodgef.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3oiiodpxk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pfhwkczo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3awyvnewq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wbnxlfva.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3dvyeqbaa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3cldzzyuh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eagrzbxk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3aiumjlkd.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ygqzoicc.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ngwdytso.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3dasvabcv.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3afxnmdnr.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3hexgiuqg.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3vpbhdexm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3guouskzn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xduvxxlm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3tsbnchth.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3cuhamtoe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3llfxufuu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3yxntpctq.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3vkfcpwwr.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ujdgljbv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ulgeiecw.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3jgamqrds.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fawomesu.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3rbjncysc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3dbvcanhp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3daubhupr.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3byzqremi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xgoppivq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3kpaaodkz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3gfaoyfnl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ujuabqzj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3zamnghxh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sualemnk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwezkenb.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3eozcjyzh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ovcjxdud.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3nsmdvxrp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3kxbjhxua.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3nlgthekn.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rkaxpqyc.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3flzbhgml.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3yrqtxjcz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3csdfolnc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3vhutpcyy.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wzszhvmf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ehsbvihs.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3vskesdhv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3pxzmrgol.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3jvzibaxh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uctuijss.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3kabkfioj.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3auhjyzyh.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gsnbifhm.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3txpgazax.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3gskyurmq.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3mmyjvyyj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ppvlemki.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3vnpkywqk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ajtgdrne.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3tptkpexq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zhhabkas.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3anerljyr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3felocasx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3airnqnaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3klxrlomh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3nwceqwzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iavdokxh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3mcmqocgh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3viyfltva.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3abpfovod.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3dfadvtco.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3utvgyfdp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3cmpqortq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3dtovlgqq.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3uixydfla.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3amqqabzh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3gattuldl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3kddujqdm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3mgzmgblb.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3buambvvr.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3kaejoqvv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lojclwrj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3liopwzbo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3pgxdchzt.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3hilstlec.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3sxhzptie.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3fauktkqa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3jjvfjzvq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3kedjibok.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3prfhlqef.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ourwyetl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3lgomgucw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3jzaxtmrm.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cjrairjz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3gsbuihom.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rotcjwsd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3zppjlwpf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3aqpcqwru.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3davldvru.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rajjreop.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3pxntxkxt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3jrrlkyco.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3isrbaxom.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ytsullyz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bwacckch.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3opmandxc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hpnzoivx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3azccvtio.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3gounfrar.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tdozftab.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3slerfbrd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fekxlkrp.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3frwwfprj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xnxumvhy.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3elcgjerv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3msrvhewx.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3oqrpnazo.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3fstbxcvh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qnmhjynt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lvlczmdf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3nbmlcwqf.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3pcqflbgk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3pobpyfrm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jbtiyors.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kjfiztgc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3iwrewqvn.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lluufcqt.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3etyzxzod.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3oyqwhums.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mnqrrmae.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3wocnifbn.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zwanvune.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3qmztdrqp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ayfbxdvn.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3btokbawb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3jucaulvs.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3eqqvmwio.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vaidvdjj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xdtbovyo.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ehlyeyas.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hkjemfna.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3meuqmnvk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3mmkkodym.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3mrhppvon.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3szjwchwi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zhbfdlxm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3aiocemtt.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3dgnrdsks.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3ioviilbn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tgezkmaf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3npdhgtpu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3kijnlkze.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3uzifwjkn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3xqnlibpi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3qtqilmmb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3glimeeut.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3iescjxcv.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ngdqmsrb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3hppqyxln.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vccnvkqg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3brievvkb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3nikltjmv.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tjxierfq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gbolgjbp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pbenzlfw.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ycggjdid.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3pxjdggqq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3fawjriwi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jzoottui.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3xqapjsvk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qqcmynlc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3qrxzrbeo.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3smviocwj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ghcnimlp.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3xvrixxsz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3tzxvxepl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bgebcdqj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3ekmumpah.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3eohctqrl.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3sgxaladb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3znoradqq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3lixltspt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3pduzzgkr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ygkkgslq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3oznvvcyj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fmchahwh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3giwihhcd.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bqzydvzb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ulgjdgxl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3mqpwtwwf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3vbiyvqvd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yzkpwrkt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ztgsmdun.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3seunjomt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lsligefn.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3gdnitard.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3baihjxxi.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cmwpwqhc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3jksvdspf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3nvqkbgpa.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3pcsnigqz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3grvsjmvb.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3yfehdaxc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xxgbcoiw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bntjrlkk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3dgaqtvpf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ykluffzf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3mkguwimg.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3vbnxtflm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3cfmydbrm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3galhcuuo.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3hmcehjut.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dhooebbc.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pbekldml.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3jbuumuda.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ybyqrxlv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3sycftjcj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3epsydjiy.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3lkfyvdgg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3saocrswd.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3setriwsn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3tmgzcvsf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3iutiyiel.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3rvseyshc.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3tcwsjcut.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kwxrjrnn.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3yfefcjiz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3otmpwaef.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vrxuiewd.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3cfjptdgl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3odqztptc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3askgdzjp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3fwlkbpxv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3dwpswlcy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3vdseibrl.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3tkvntwek.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3mzrppiio.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3srchhkgo.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3mswwoxfg.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qebuzjmx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3qhjlgdgl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rdzugtjb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3iqrsdazt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ylrhlchr.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3pmcpdeak.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3npjrusks.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3hzgtrlag.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3tvuybhzj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3gboblmxl.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3nkycmahg.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uqolfpff.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cndkrxhx.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ayegzyol.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3babaptsg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3frxtqomo.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3agbuoljz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3itbpxsfi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3bmtbfyms.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3mgjzvein.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3bbehrghl.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3hmnewlbn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3esleqjvz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3qmftitbw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3bhircyhd.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nulkkvpt.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3nipxjkyc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qkcixdzq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qxmorbzx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xozeuatw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jkplwqty.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3seqiofsf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qmbheepq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3efbndhde.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3elbkuqvy.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3hgvgexvk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3vzrewqeo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3duymnaxf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3efuvrvnr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3iaejyoqa.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3cgzcwwxi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3dsmqlkeu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qfyylbyy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3sheomqhe.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3nmtaslgr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3jcpfeelh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3sowbowow.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ocsliuru.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3rrzbwivy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uimvmtqf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3egegtttt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3gjyulfmu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ahgvfvmu.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3rdpemymy.html


<!-- 参考信息 -->