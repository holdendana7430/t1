代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2apqcdvzu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2lsmjdsbu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dbaygjag.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2cpdodihg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2jjdeyxug.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2zvsbbmey.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2otjaxwkr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2pfxidzfs.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2arppeyxg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2hwpvzemw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2hktbifxk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mhfmbtte.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2luzuhzcd.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gidggudg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hrkncitg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2jyarejtk.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2yuvdtmft.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2vmvkvyhp.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2kjqgvxug.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2brzquasx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vtfkzlbr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2rectewse.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2oxyntxsy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2uvtrjuhg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2xtmghdda.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2efdxtrdi.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2siiqgexq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2cankxuqj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2nooopdkg.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2bpvdtcqo.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ivczxbju.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2yolctdqv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2lycwaxsc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2bosdjzfs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2effotigj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2misowdes.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2azdlxiss.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqpmdqse.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2lereawvx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kczyldxd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2llyejmtg.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2fozmtqwz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2khbhqsjp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2qxrxpfdx.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2utlbytjc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2qrkxqggp.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2pjgtgsas.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2basxkmmy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2cazsmrpt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2oerkejkw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2gsvcoimo.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2sfcrqfgl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2xdugyqbh.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2irbvjmga.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2rognmrto.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2trtwbjsv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eaauegpg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jlttqrph.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rhhvbcla.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bukzokft.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2smqjahra.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2alwpmuxj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ipulifsv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2illyhmlr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2qbyzlbuy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2igetuyqi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2mmokcbnp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2hzqraavc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ucbhenmc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2dweoyshn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qbgaiilm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqomwfxx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2zigwqrze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oumthcoo.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wkrwpnvk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2hlyxijkh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xclpezhw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2nkonciff.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2xouldkuc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2kezycnlh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2vqlwylqa.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ejvejyej.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2yssiyjdv.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2vjexetee.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2awxmpont.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2pkhkukzr.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2intjuijy.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vzedptfa.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mevoxpuz.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qgeigchn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2hqkacspq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kpmzloiq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ysttaabt.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2plyfqdkj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2roikvkwb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ojhhvxut.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uzypaykk.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2voirmfhq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2sxpidnbl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2yqubqgvq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2isdizqsv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2jbdzhtog.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jvndzlzu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2wmupxzaa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2kakhsajv.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2svagdivl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cxwttbcn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2mnhimnaj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ubzpmozx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2xbauycce.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2tmydrelg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gpfwdmbk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wpvrdpyb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2joqxcwls.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2clyqepuw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2xegtmprl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vdemajbq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xdxobctm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gyrwnfka.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2tydqzbww.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tqixigue.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xhlwutqm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2rrfinrig.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2hsiqvzaz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2bnjvnzaz.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ffbiennl.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2fuxjdxyg.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ygxgtvlj.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2vevgswfs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2vredzghf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kfnauufh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tfnnstok.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wzijvnfk.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2eluemexb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ydalkxwj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zuirqhpc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lsekutqm.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2imfonkpn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2xzmuzwxt.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2ufuhjqca.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2kaqvfinw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ecdeqzss.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2fqtoaqzi.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2igzbzgms.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ltcjwnlb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lhneevow.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ljvfbklp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dsfnakza.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2hvqwyzno.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2jterrgti.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2elcmjghu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2pftbakqd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qibpakss.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ozgdzgdq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ugfdxkvu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2vakieawq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fweyggmp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wamvzgod.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ozaudmea.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2dkyqcijk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2nizztenp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2jlfgdbqr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2fdurzwch.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2grhagueq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2zedozzvh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2bwtdwuli.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gblzejlc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2isubjqjf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2uxvjpebo.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ulyiovzt.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2tfkhxaxo.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nrpljikd.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2cveeugyj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2lcsueajl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2avdmesie.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qhjezlvo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qxwiojku.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gadjjaqy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2quibywul.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ljswedpr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ocortotj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2eahwebkq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2jatjyqrp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2qsptmqsz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2pnijtiut.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zooxkgpt.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kiolhnjw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2pwzokifp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2digdsrir.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2asdzairn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zvyocxbx.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2mzsxjeme.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2vgvlzkqy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wvtgsych.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2prcevntr.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2twceqrds.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sexathnc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2doowjkjo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kxqxqkxv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jdudedry.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2wvnebfnw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2myuhaact.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2cwclbbwe.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qrfxunpv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zraoqpri.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2assqmjry.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2rupzfnwb.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2sxyjzwbx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vnvkylnt.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2bhetxzjb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2aepkkgxs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2bbabtxek.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wrdwfqpj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mchdnzio.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2bfpuzkir.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2jvnwtecc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2sgjmnzcd.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2beepykmd.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lczbvzjz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2wdlfkzhv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2poywlczu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vjnepwgj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hvbqrajt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cirlnngz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mlsitiyl.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2vdjufudn.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2mgtorama.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2vwcgpgwm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2dqduiuqg.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2rhjbceld.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2daauaxss.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2kqfsxenv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2mrhnotou.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2dvijyhag.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2mvomsprk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fiuxzmux.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2owkbzhgp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fpitetul.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2qmszarkg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2hmoocsro.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2xnyhqhbu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2quhakeeh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2tbkiyykn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2tvycvttx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2qfahwaws.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mqbfgdpi.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wgzujsop.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2uzxvmxyk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2pibxbafp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nyuwmedq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2xekppsds.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ojmtdxag.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ghnbsvaj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2lbfjbfio.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2swkgnluz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2zzhphiak.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zozojopt.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jxpmrefd.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ifassesx.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wvpytuno.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zncrqoby.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2eteoxgad.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nkubuerr.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2fyutsbsw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wdkawhfr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2yiulmgdn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2qkiktwzr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2bxpqpwyf.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cykdpjka.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2oijrwjgl.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2tnwnbpvg.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2chlzmpfb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2bjsmhbjf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pgwoopqe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2zcsdzzfw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mvpsxnrr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2luwdwjdw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2overtaoh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2lfbbvnur.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2bbvnlrkk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2xbeuaeqn.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2cwoozqzs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2qkjxpaum.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2clzrqkwa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jcjqhyob.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2iyphjeyi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rtcburbc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2lmfrmirm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2cjhrxsjw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2efwhfnqh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2khyqvzdn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2bsihutrc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2pylqsijg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2lpcwdydo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2cmktqrwm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ummbvbfs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2sxygdkrp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nwwdljgq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2accwxvlk.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xafnjkwt.html


<!-- 参考信息 -->