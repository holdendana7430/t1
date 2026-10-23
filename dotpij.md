代发 wailian999

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3edujlrfv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ozkigykj.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ikqiwtqy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3fezckezc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3mukbfdid.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ktgzhpru.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3xjoodtuy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3pbovfufd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3sljnfsri.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3invjvjao.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3fasaeymj.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3amgjltic.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3lnajgpxo.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cfdsbbqe.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fxvtmncs.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3nprotvlh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3xujycpwd.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3hpsvntwx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3wntlyjrz.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3gaudqytm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3gedfqhga.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cluoszvp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ybbyrtxt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3iwstxnxe.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hmqzanyr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ajewpooc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3qhplhfmn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qyhqrsnj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3aetkzokj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3qdbnrfml.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xstargue.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vbpbbuht.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3vprfujic.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3yuhibfqs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3vnewgbsk.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dllohnxt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3lxuwhguw.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3uyuaaizp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3aheuvhkh.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3zgluhtki.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xkjuflap.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3bxrssxxl.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3shhhasmr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3mwzcmkbo.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3owofeofe.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3iaxnbolg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3lrkyyrlv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3scowbube.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3vpumklme.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ddvjabzs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ydmbhhbm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxpktofo.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3acjyizie.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3hqcacbzf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jplodfyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nywzxkcw.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3kxukdkww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eijcteja.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qxfxqqwy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3dqapjxkn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3byszylsj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mwksmrmb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ifuwtyfr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3idzsgmhh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3yajcqubu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3kfmwtedq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3elveygsm.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3rpeipsnc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3wpicslbj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3cndsumkl.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xwftczhf.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jysezdhi.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qwcjqdyy.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3yhfldlkl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3dkxokrro.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3eblutjdb.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3orqazuzn.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3dhxhraks.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3lzgqtdlw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3qdyuntpv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bxmsqatr.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pwhziazy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3eqvdqase.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3yaaymdpb.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ghuveryo.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3enykjknv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cbjnyrpy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3cobseoxw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3lbnxwwsh.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3wyhsenfg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3eqbeznmo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3kdsuddow.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xemccifk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3fyobgzgj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3culvsqbl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kaippslv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kqzghmkk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fnodhnia.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3isfvmaob.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3hroawlly.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mjjdugjs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xrudbvzy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3izmwxxyu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jkdrmany.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eihgerav.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3tjdsvbay.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3snxlhuny.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ujolvkxr.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3hbblsipa.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vmfmimmn.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dkiahzck.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3hjzrbxll.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ehbrxjgt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3mabsaujq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zubdngup.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3cerlwlyx.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fmopjwto.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lraeljit.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3dcxgkwkm.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3zqnalzzf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ojuogcdv.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3indducwi.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jidzqxlf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3anqwytmy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3utelculm.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3fpejignt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3tvwrffiv.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3qzoexoau.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vtoemutt.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3goderjdk.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3bhwraunu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wkcmymje.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3bqvudxsg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ecnlybtt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3opeiymgk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ubgsvfsq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mdiinvah.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3goxfgghr.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3xeizeypl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3pixzyyif.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lkzawlnx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oqrzpzam.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3kmewebrp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3qjmkjhlx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ebdmoogf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3eiihtjvw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3zmrdirty.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3wlfpugqy.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3nharvhea.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3jhuckwsd.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3pzlmzcqj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ebqkrhdd.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ldserlgi.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yktzbsai.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cxeklrzl.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mhatsvor.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mosjjdgx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3gwphkzmf.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3nqkawsta.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fuybtqfd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fgqkmpzu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3grhdtxdk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3bsbpdwya.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jmclpqke.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hrgbgclf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3layxupkj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ktludeyc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ohfexees.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3swhrnphy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3sowvlngz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3hheurikk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3aakdrqty.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3zpdexoue.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3juwazhtw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3octxlzke.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3lsdepifu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hqmvhmqb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vubqaqft.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bfniqayt.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fnpnamgw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3uspmrgqb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3wodrkanw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tomvrymk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zjmcxhjs.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3oudohpwk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mckgunvt.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3awpzdtrj.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pqdeszaf.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ntmtiqkb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3cemsmfsu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3akwhvgod.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3hzmpordb.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kmgnfokz.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3jvddiwgz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fgfstjzf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3oemdcqug.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3bodkgwgj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3dfybmdda.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3gkcqyktn.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3htbcpcoz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3bqrkheel.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3wtdbmmty.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3cdpqlgug.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3muzzidfa.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pcplcjrp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3xcpguwon.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3vryuaiuk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ietwnrao.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3agggaqxh.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3mgxuvmqa.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3epexlpqx.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3jmeznevd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3yomtrijm.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3hlpjunay.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3tdxwyhbv.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3zhdxnlst.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wekkorjb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3wmpxajiv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3eetocept.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mphkabvh.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3duriadmb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wegafprh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3iscruesg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3aawohkqc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pfjyelqo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3bojcqkku.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3vavmbzal.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3qtnvcoio.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ubjfkkwh.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dtjyngfs.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3beinpijj.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ybwveyip.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ceppdloj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3cxxmeqmb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3nrgqkflm.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3nqdqykal.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3fmeuoelt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3vbqexlpv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3fzmwprwz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3emfmfeii.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3cyxzgtlg.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ocfobqci.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ceoyvhan.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mjjfkeze.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ajytrayg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qjumovgx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tccitwse.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3hakjehpo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ywbdflyy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3pvjqytvv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tiqzhlkx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3fbbjtwwf.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ccaygaql.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3crztvrou.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3srrrqayv.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3fmiqluta.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3qtgudfup.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mcwjmueg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ryrazfwk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jfntbaeq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yehahcmd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ceeqrfwe.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jpjgnrrd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3pwwqjfqy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3dyzyqhhm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3utwklgkw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yasndpmm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3thcejjwi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gzuyspbq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ietdpenz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3sirzvuid.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3xtxbntpu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3esworbjk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ztdwpbfi.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3npntggfb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ahdbjbxg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3cobxdryn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3csbrimfj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3oqzuqjfi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pmvsrmmq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3fzldfrzt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3myqqhckd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3kavvzauu.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3knjoaoxd.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3oyxypbjr.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pairvoxc.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vghglhga.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xckignjh.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3roceaabo.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3vrgdwkde.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3pojannfs.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3prpmvdtx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dzublump.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3rctkuiqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ncxmjcfd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ekydzdlh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3wmcoqgun.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3swsolbgv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3hlgcdtzz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xwcrbhoc.html


<!-- 参考信息 -->