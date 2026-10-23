代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffnznujh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pxzxmfvn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mppzksvd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ueqrpfda.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3jnuqwdmd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3xbgymugn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbdkfaob.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3qgdrirvs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3mykrscbs.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ddndnyoh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3avemxcmr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ifsoqpch.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mfnumkkr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3fpyciuoz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3noxmfesj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3lymgygjd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3kdbxrayb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3wphuwpry.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3yxpikqqm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ndjpevhr.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3gqaevrmo.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nltcbnws.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lbttwpsm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3blsvyhsp.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xpmvvogd.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3bvzqcdti.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3vldciyuk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3hlxqoisa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3covopthx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3oquuwpke.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3foxwubdb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3igoasuxw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3afbtpjyd.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3pymnjhet.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3qbbubdwz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3cjbtdicg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3dctkflqa.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3yrtzswry.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3egtqsuzt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3zsnsvaql.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ucgrltio.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3hodwzriy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3pwxryvpg.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3gwdjsvhl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ofzczctw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dlvvwbqt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3adfqxiqe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3boddzdba.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wwrtqcnm.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3iveuvfdn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3qxesriom.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3rbtcecgl.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3bnwlhuxv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3aiflljxu.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wismfnuu.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vfhybzss.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhtvvknh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ubkfjvur.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3vcjgqgmy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hlrnzive.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3gnfdwany.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3lnlblkrx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3xwtziyat.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3qwiytjzz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhnnwfyk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3enixkvjz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3lepyunvv.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3nxpnnqvd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3achxcgsn.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xpgfstdt.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3fwgatnzx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3aclmgpqi.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3nspmqoyt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3nnaqjrqk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ywavdpjd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3chmweynw.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3uchydsfk.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ennudgvi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qnxjbwsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3czmulofd.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3husvxotl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ufiidsfe.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3dmqatxfc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3eojtqtxg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3cnqbrdgn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jgjdirmg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ozbyadvx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3olosqbfo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3fstiofql.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3fepbdbnt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ovixnukm.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3bcceywwh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3scseghfx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3appdcawu.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uzcvngcd.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pufjfbzt.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zrllwacd.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3oyavlyax.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3lrfcngmp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3trauxfmk.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3lcpkjpqx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3iedgkkhq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3digwkjji.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3zwgvoyyb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hzcklwmj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ozhjlrpz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3vbxjbiuh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3cveqqmlo.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wazqguwp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3wuoclpwt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3xnpdnlcx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ammoodpf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3lxirxely.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ktsnaevg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3kuwiyszz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3fzqdwiud.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jyyduyof.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3nmedrvuq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3pdygijci.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3arwnpydp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rivboado.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nlnxesit.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3gwfyzghl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3mxvjrdnt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kdotqnmd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jktbeqsc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bwlupyhd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3nentzgfo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3thfeidjt.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zaagyzit.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3hmiaetrz.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mdhzdjhh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3viezykhf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3plxqrykl.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3pcdrpshz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3hqnawgwh.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3fhrvbodd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3dkuzeewi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3wghgmchk.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vqofwoyy.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zrxdimxy.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fywpwcdk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3taeerinw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3exggvrpp.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vzzmwscz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3fqvcujnb.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xbcynxxv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3dqzcnvja.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3koidzpid.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3gdudpjyv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3gwhnzvqq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3pqwqwimr.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vtkgprkq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hhrnizkj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3nzydwgdw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3uwjtmrvv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3hmmwmqsd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3hikhweio.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3wwsnxlfv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3lmjlkdtf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3naqmryyj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3eljnisbq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3yqvsnjhx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3fhzokdbh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gvraokyy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pmrdflbr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3porpplgc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3whftjcoq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3smmygmep.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3fgssitzw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ykuhijpa.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3woouejxn.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3uynkcbzm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3oimavqtx.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3wslkthyx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3phrdpkhy.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3byjqinho.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3rbjvsxfk.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ytqhljiu.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3udocmxrf.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3lvzlxaec.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ngggiikz.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3xerfbotm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3eqybsaba.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ejcqcbzq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iiizymai.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3sskaqtbs.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vjufnolx.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qjdxfftu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3hbuwtakr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3gaximwxb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3feurnzyn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xihszjds.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3axendmol.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3onlqzfyg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3jjchjhhg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3czaemylc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3iodhoztp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pcvnslac.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3iuljhcht.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3sngobgtc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3twgdrpuh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kllxksqk.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wzmslvzp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3uhgojsmd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3euwxmluc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hyqlvgdb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3eykcvepp.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3zwtlyirv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xxnvpjvd.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3nytplrhg.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bkbpycyn.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pqyrpagu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3sfyebavr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3hoieuppg.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3impbrklg.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3xgsctkuu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3buokourq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pfhalria.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jvvugaro.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3gveeelwl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3higjrhan.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3jcoanhxr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3gfxqwtew.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3nvtllqyb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3rpprjxdf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3qoimdzqk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3puiwhyjh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3rclitycc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mamijpvb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3tldgiaoj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fpdwgazd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ankjrvfb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3azglinzy.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3mwctnkjx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3jwrbnhnd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3qqflczaj.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3podwkczb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3wumeligx.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3gdmmslkp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lxyxeuuq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jlmhgxmz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3rfekybhi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ughaitak.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3uhbbchft.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3xcjyulyf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ykybimrt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3uvfduxni.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kjascsvk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3fiqcggkp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3rtdxdsyq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ygemkvxx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3kxbcykgj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vgtobpjy.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3glytolrb.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jnctdhws.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xkweummb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3sijbchhg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3xdzizjpo.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3tftjjjcd.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3stgiknzo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3guqtetej.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3mlnpmcfw.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3rzbpvvxt.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lhdjxyoa.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3txdcmcvh.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ynjnacvg.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3irhdndvx.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yiengplb.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wfkozgyy.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ongrozvc.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3rpzadzpo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zuuixlxe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3kkuiscnj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3pxhfbjft.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3mmxqsijs.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3vsfbboda.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3doosoymk.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ukajorko.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3esvvezjz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3alegfbhk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rzeqizym.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wjiqsvdq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3rtbzeakv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xyjzvtwp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3jmhrqpxx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3oywmrhfd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3uaezycau.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3rswwaosu.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3meeqhcuh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3twdfhpws.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cuprchaq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3edkcszii.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dgnahgdn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rlyxnbon.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3xbzzscyg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fwikhhfr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ackvbjqs.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3wyiditcb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3epybtlka.html


<!-- 参考信息 -->