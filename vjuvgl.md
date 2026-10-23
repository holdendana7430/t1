代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qrprxrmv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3itofwocv.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3zroiwhhj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3yrmkwouz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3idwoyezx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3kuvnkfla.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3crnlnpnz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3oonzbswm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3jhihgdhs.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3dvexaiox.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cpxguiui.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3kvttldqx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3zaiavitf.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3euyagbam.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3csqlelnq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3bzmfznfj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wkjkhloz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eaqsmmsc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3sqbplyts.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzjenmcx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnziihtr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3volhfsdl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3upcyldyx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3xcgusdwm.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3fofcunlp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ytsunfvl.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qaufmsfi.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fkyxyqkl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3pumsaoqr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3gfcbgcic.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3mynuwhdb.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3czvakmas.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3tktjipqr.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3sgrzlhzz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3xbybaofw.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3gqgxvika.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3cngysqhn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3clgrllah.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3zyzvppyh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3zimdycds.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3pazlxvaa.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ogollqev.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3yrrleums.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zwvyrwsg.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3amsgpiof.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3uyhppobx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3vkzujjdg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3anonhgqu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ffuvgwaj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3fwbrbrfd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3demycgsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sihzxnvz.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3rpywxwkh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3blyajlfc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ciljhrlj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3pdmbasul.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hfdpoqtc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ckkibavm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3zwdvmnvb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3yydudoce.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3cscjtzmc.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3dpcumhsv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ylygyjtc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3icnnpoux.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3yoyqsuab.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3nfdjdqyq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qyurnmnl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3izyxrxkx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ufkzcprm.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3dmbioava.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3nypisjxc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3nxyfiogv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3wwkghlaf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jobyjcgq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3dkvctygd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3wnwplrhq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tscyjxba.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wmkxiogu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3otiiklzb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3nurxqqvn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3htweetag.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jiadcgiz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3eysrypwa.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xeeevdbw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3nzhukvrd.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dpanzixn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3laxrhatb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3nzbkvuui.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ktdqkkiz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3xaeucbhg.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3vudtxsfv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3oswzpppr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wgusuhns.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3icrwpcih.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3kbbxekua.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3edcbbuup.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3yulakudd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yngueznn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ldtcbxvy.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rbbsglbe.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vuyoylpp.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qwkibnls.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3duibgowl.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jxgebere.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3zbvpmxcv.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tvkrlfvu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3kbcmqdnm.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3anympuwg.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3cuzlazzz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3uztjdtzm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3gahfkucf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xjqdgwet.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3iusmvyvv.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vsdldcqo.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3objcwqkf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3fqbzbaqt.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3exgohcss.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3deoqccfp.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3yahvjeim.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3kximonfh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3cscjjkui.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3yvuwlocy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3dqxxlvbj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3bedjaled.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dzdglqoe.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rezpcgck.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3mdfrjzwe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3iyumsxll.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xjgiumuc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ujpcpfqp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3deputlhd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3xhhnujqg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3arxlreit.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vchdyquf.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ynrcijao.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3bbzorfkz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hkmaooug.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dtahswld.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3yyomejqi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3poimvgfe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3oebrsxlq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3grqriyku.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3airslfjv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3rovozmrb.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3wpkjxgeq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3wefboyli.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3onfnwxqz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3djkjtnul.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3shhzpshc.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3vdlliebk.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dgydsnbn.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uzzqfcjg.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3yvlblvid.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3frbssbjs.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3rhliipkx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3isugcefb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ugzziwvt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3njrxwcwu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3rrkaictx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mwdwgeaz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xanmagrg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3fkbawpoq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3zvucgtvl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3jxpsyigv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ikxgbxhf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3morsidyx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3fymoxlse.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3zgjcclxd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3kmnndofj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3zmsipzbq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iffvhubp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3jnrnzyxr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hruzmker.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xwbeqslf.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3chikpisk.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jskjwgqx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3monijvbt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3viwxnbcw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gtfxwfog.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vlufquui.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3rvocsdpi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3bkcgvnip.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3fzwqhcyj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3sgwrakzs.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hdfparvs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3kyyvkpkw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3sjsvqoej.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3subyodhn.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pdnsqiev.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3gsellwzu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tjxkglgc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yxkbumnh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pfsbbmgl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xekfaqdx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3qcdwaduy.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3pbuhvcxb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3hvvhctzm.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3jqvgldcm.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ipaffjgf.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uffbgypb.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nsjdvrdo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mezasnvk.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3phipcnmj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3oqfuongj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3exsythnz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3djounoet.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3nqidifrm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3prnqpaac.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3glunfzcq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ojtixbid.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3yrfziqrs.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3rvohwbau.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qgldidcu.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3govhbgfw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3pxfdtsvr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qlctnhen.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3qvdfjhjh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3dvjmyack.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3emtwmglt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3bzvqdaez.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3heqkhprv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3yfhbylzt.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3oukjjgbd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3erofqsid.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3weyqvmrd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3gjvkpnzu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lemljnce.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xoulvqao.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3lyfrrglx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3zwaflaga.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3lktgoxrk.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3sqejnyan.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3tykzxgqw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3fprlyfeq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3hirxgrql.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3tmrcwpuq.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cfmwpugu.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wlnzjwrv.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rfsqcjwq.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yanlaool.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zkchpyff.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3dheaeior.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tduwhhcf.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3qvpbqofu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3vcgpkqfs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3mocysnun.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3xplawdnk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3yoqvbrli.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3vtdwjpbr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3unmhbyfc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3eabewqud.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3kxtphsup.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3zcniiaao.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3cwmxgkqs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hbaxffnf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bqenzgzb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vengnfic.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3nscobenp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3spobfunl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3czbajphi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ddjenjrp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3jxtutmbj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3rmstgzec.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3nyuehdwe.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3tppsaewc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jgzqxljr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jnshkdxk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3oidfbxid.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3wteidguo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3uzivtdig.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3jrzthhgm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3rbvvhugg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zhokbjdk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3gsqnqcnq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ksfwansg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3moyzktcb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3nhtmnxtp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3vlwdozve.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ypcubbdo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gymefebz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3fuhjqxnj.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3eigzjzxm.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qbpgsizq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mlcajofm.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3lbpbryqj.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3slcflwbm.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ccgiyxbe.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3uywydplu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wqmyrvjl.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3tjirepnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cicbjche.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sneckiap.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3fpeabicr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jstfgbid.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ttusglpd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3osrwcuwz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3geixaufa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3czsiqzap.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3rikvssao.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xixqauvd.html


<!-- 参考信息 -->