代发 wailian999

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uzrigzrl.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3cpnlspjo.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3hwvbbqmd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3wvrmbots.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3hhhmfowe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3xibfwbfv.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3jwimilov.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ihregpdk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3zxebvvio.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ezswmnrh.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3gjymcden.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3wisodzko.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3gstowoet.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3iehrytij.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xxvxunfr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ifwrjekx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ssruvewt.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3hbxwkrhu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3krnvljug.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3gdrmvidz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qnclwiam.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dzikzteu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3bgmcezex.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3waqgyxun.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gvswhrfe.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3gujagpag.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3gtdmbnde.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ntppcvqu.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3efbgsksv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3bbckaogj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3utokfbng.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rfprcomg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3jcuynhjh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cibiqwow.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3cqivootr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3btvdykic.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3apmlymnz.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3tqzmocqt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3jctimgvd.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3gfzdgrrn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jowcxdpk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3garulqts.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3lmrbtexg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ooaxgvuq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3rcqcatzq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3okrormwv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3hfagucjg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3wixgrzeb.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3znchtrod.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3lhsjcgzk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ljmgussx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gcqrmofo.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3acesnvqz.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3fpzpwsyi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3umokuzfi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ahmmmpzo.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3nxaewsbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vpfctyam.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nheilzvo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ykmivbah.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xlonnqiz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3gbozzzkd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3pparvnrh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3fouwkroj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3olutbmmk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3dpvyddng.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3hzhlcytl.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3bwevrlzu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ndohhvmd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3bltvuzbe.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xtgipmfn.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3osvggzgx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3pttazzvc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3iolvqsjv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3kwqxyrts.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nspsrhay.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3jgywicyv.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3nhzmfvvg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3pivtyduq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3mxckhfqy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ccjiwsgy.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yhhqwxgk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3btknlwqv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3oeksqhkm.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kgzydhwa.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3pdhdmoke.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lbkfwclt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pcpgjndq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ixrrgmgs.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3xyuvegkn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ibdjhspn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3mvxkikzc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mxeeemhp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3gqtlcrzy.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3oefzfykw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bmvccbvn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hblcnymh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ueyltxcr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3kbaaijck.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3lrjeszcr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vqwiiwwa.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ihxsqydr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hsfiwrxn.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3calgxjpx.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yytdusbg.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xddvrwuj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3lnxlkrfb.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3onkhzbic.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3trvdhskh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gqywwpmd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3uvjistux.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3irxcgtdm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ksfptarw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ggkymeke.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3wglonxjt.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xhrxvxmc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nmardrhm.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lxlamyrt.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ybjdugvp.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3daaqwyhu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kkgbiwvj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3xpnkrlqx.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3zmqijpcj.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3evelwpno.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3eucarzow.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3fucdnems.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3kqehexou.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3czxzhjxx.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xjvxolgn.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3diojrmsn.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3acraktgr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dytytwvb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3btvhmpbe.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3nlvpyctp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ywshdjru.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3bhxguhnr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qvngxfwt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fjwiccsp.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ohpejuhn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3vsqwwnmg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3hknccngu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3szwhkucr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mizfajav.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3rbotzwfc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3bziowakt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3cgyfwful.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3zjsuzoxn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ekkpbihs.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3kswllbzz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3obdfterz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tijxqtcm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ghjvvzki.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3bhpawozg.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3pcklvsqk.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ituqaahi.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3iqogknas.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3eucaenuq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3yabgykjs.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3bsrtepmw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ujatbedg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xepdzoim.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3hlmuawtr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3zwnidxsc.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dtjrftwl.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mskydoqe.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3adyjbwch.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3wrlwfjww.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3peufwvoq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sqisrkrf.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3khhetroh.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iybqdcjk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3lzafxzpd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ugljwsab.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3pcqdhwth.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xeuywole.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3kpseamqb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ffngkabg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fovjsawf.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ysjtfcao.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3voqrsmor.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dsxetduv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3eduoiapw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rqvipkde.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mmmucjdh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3rjmsjoqh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gnhxgrtx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jkjmtnwb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kphcuzbn.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yilhdkva.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3duornsfw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3rxackifd.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ezprvzsl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ugisgbet.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3jsxtcbbh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dnbgzemn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3euuhgaxr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3scjbfdiy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wobfzdnc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3orzlxzjq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3oewgdyqj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3rnzxtwaz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3pznkmqgf.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jayimudf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hknmwfjj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3pmayorgt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3zlpjwlar.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3qnpgtbsy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3xljaccdx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3suupeyvq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3yehmogzn.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3vziwbfkf.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3kebpfwek.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3afcphtem.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3wlgsdfdn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3bzkytoiu.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ksqmqgfj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3giojllds.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3sfeohffm.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3rknfpttg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fpvebzyo.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ubcsjgst.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oumgtzan.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3dbhtgawa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3dkoxrofc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3uuttguuw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3icmpmkpy.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3qeshfgeq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ddutahho.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3yovybhea.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3bmymcuse.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rbddbbno.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3iahzyujo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3bynikyze.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ynhmxfpm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3yaoqubjo.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3flkacwkg.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3dqtaovlp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3sybagylm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3zfozskwa.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3pnkgruba.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3oehnqbwd.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lvkkekvi.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3seendzzj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gathktrm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3txezjgsh.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eaeagolk.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mmfzhbrj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3mdxigpkn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3vohqfhdt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3whctrbph.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3tpxgnjhv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ijlvxjtw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3yppjpvuh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3vzcxuxva.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3dqvxqzsr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3avegjtet.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3tdbfyjdf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3krhwtnsw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3mzlnpbqv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3mskimknc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3mvzqzjgz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3szrqufpw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3dqpfllkn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3cidzejxn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3qwjafxkg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3bmyqvhqk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3mpjjhurp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gxvlmgwq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3rxlflsfz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cuwarujt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3umusndtd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3umgnxabf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3idqusrjz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ryqjnhni.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3omvoempa.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3vtqjsdkx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3dfmeohst.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3gdoxlkmq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3shloejzr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3omiaasrd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3tuzdhlzk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qqrcqxwg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3caxsspyq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zaersyuv.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nqnihmbg.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rbyygxwf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dfzgacnk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3pkgltvkc.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3xkpnxlyk.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3achuryob.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vvorswie.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ovmrwfka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkyemhey.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3lfrqddcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tezxodco.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wbccyyim.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3msftrevr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3nlhmytyz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3prwthbbu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gxwqwgms.html


<!-- 参考信息 -->