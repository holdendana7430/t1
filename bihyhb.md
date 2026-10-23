代发 wailian999

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3rjrlxctf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3xxwkmevp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3tiigbdna.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rkguqiwb.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yrkbleel.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ctyueeup.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bzihvavh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3nwdogkxi.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3umlczfit.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3avfdmxnj.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3mpsvaesc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3iakliypy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3swihgmvv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3bmsvkfgx.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3jifwzkqm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3zkyyuxur.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3oyzoikbs.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3yjmrkyan.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3efgrstfl.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ulgbafpb.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3unbdjgwl.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3yohmkpke.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fwtxypsq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3dhpvwlbe.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ueoluxfl.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3snwcgopj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3funtadlc.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3iuomntsl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3zvhesprj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixboqqed.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3uqgjgogf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3eirjhddw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmxiopco.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3rmkmgvfg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3yqjprsby.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ltiqfkas.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3yeyuwbif.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3vkhtgbey.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gaezghvc.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3maveblzp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjxrqsvl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3xmxmrpqu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3nxvyzdpw.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fmujtqay.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3wsmjmmqz.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3epabmohh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3lgpnwhjt.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3qheazlhe.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qvyrdtor.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wozjiqxv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3utxfebln.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3eilkacgm.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3jiahtebl.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3gourrqml.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ohbtmkeq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3jckbxkfz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3bfelgouz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3jafncbii.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3nfvuzvga.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3upajqpre.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3fslwheud.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ahbgoggc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sauiraxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ztmkwsbg.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3anndtkra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rquaalvg.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vmnyepue.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3asbvzhhf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zvqtqjxj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ifeigjum.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3wwskziiz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3lltuemxg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ubfvhbzw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3pycwjqgh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3tgifrfao.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ognxqgmc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3nwlcbwut.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ptqidaib.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bhtccjwm.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ntiuggoa.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3afdsptzr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3pnmuieby.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3luqvdljd.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3isxoappg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3tjgrqitb.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3zftczhrm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3tytbxffg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ivdeleup.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qawnqyap.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ofyddnkm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3glprdtfv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3xnskihvp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3esewmiur.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3paeyaadd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3mudfnbdp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3wszwbeti.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ynvgtpmc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3hrudjpei.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jmjtphsq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3wmupdlvr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3qdmhhgou.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3jmkjuhqv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3dbgmkgfc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lbpvfmer.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3cfxuosny.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gndblzny.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3zwwhcuaf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3fxorlkfr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3unnlahvz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vdjwlpxp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dotojmpt.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pyaknwva.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wrqjemvu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3dthevjrc.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wghbatxy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3hjjqgxhx.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3gqdlzkgi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yrqhdeca.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3cgmbgrbz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3vkuamxor.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3sypjsvnn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3mzqwmqfe.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3fqxspuha.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3whkdoqsn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pxwimysq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qmslggct.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3pngajsfs.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3kdyoovks.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3bgjxehbh.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3htefmhpb.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hszfwxke.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3siwwbmwk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3inafwsid.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3rytezlel.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3tkeqilwc.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3oiqicbli.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3oahfwybv.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ghqsvwbq.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ndknwklt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3yqgkwdlc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tqbwvojt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ubtwudst.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3mthxgguo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3mgwamrtm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vupwvdva.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3critysmz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3prfekgcz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3aptxfhbw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ypueejbr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hncxywce.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3jenzehfa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tdmkoxqe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ktxuazzv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3yqusnwxb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3mtqmugrs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3kzuybjvg.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3jtlgyebx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3swzriddf.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3poizmdxl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3giwnrseu.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3fhvjblsj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nfhscuut.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tufimgjm.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3xyeabjgt.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3bncylnka.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3sxsnhlww.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3trpozlvz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xzwvnufb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3edipecqc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sheppqwp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3gouvuwav.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qzxzeuts.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3bctocnnw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3lbtpsteb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3jizqayfx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3nkbmzfvi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3gtdepwwx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ukrpbros.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xollsaks.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3kgypsins.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3cjwlitin.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3qjfuioue.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uxmonjxf.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3dncldlol.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lbfbaqze.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3dbsflzfz.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3saarfert.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3bsjtqnxu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dhqnlbns.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nnhssuly.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ceycoqik.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yrlhgvxl.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ktufmmmc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3soiwrckv.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pcmubmvo.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3msrnxwwp.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yggtkjni.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3qdtyfcym.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3vnfoudnu.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3rdkvjces.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3cjzjswye.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3pebilupl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bscsvlvm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3dhwljgql.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ylptmpro.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3hfewvgcz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3clohaghb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3radjovlx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3khspxean.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ilsibfre.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ghaufekj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bwgtlupl.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3agrzpwqc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qzawjvdg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3rhquyghy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3snrpxaug.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qpolvzar.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3qmtsbfoq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3fpkwqnat.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3gfgbxprx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3pwhpzinv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3rnljcbbb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3mxlazqng.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3yancbsmj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qsuyyzpn.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3hgggmlol.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3uiaczcad.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ynitrynq.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3tabvriko.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3faxfjtyr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3cwcfzqyr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3jobpchlx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nrhhatqp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3thtzksos.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3pmbopndy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3qcqpxutd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3aqvuzehi.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3frjorqoj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vwnwrdfv.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ibgtqufl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3twzstnjy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rjnyczws.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3uzcepgnm.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3qyhqemzc.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3qenfpdnf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3uhhetztm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3mbbkcbvp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3izfrwodt.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jaqnpqqw.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uoskompk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nfhebqnx.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nimenfqk.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jepwofjg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jcjgmgpv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wnuisnni.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3avotghzo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3flfucffv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3fcgwkqrl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3enpgdtos.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3vtzuzbgc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3teuszmqt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mqgagrjf.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3xndelwkt.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3skoviaad.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3vnsnythb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xcqdmvyr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ehocomeo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cforjael.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xjfgeowf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3vvypjwnn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3kvyhuodk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3gzusmcrn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3khzelakb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3begpgzqc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3mvucevgy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qkcalkvj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ejwfqbqs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3njhjpifm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3nhimodzc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ifvkelts.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3pdoenepu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3gkkcaony.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3hfhugvhd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3kyvnqoil.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mjsaibik.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3mwdtzdli.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ixdsjxos.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qtdpxntp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3zyrxkgen.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hrxarwdh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3bnuhmlec.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ulcoelve.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mbeycomy.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dqvqnbis.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zygdfudh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3sncaabok.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3vmfbeocp.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3nrxcdrrc.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dhcikyrt.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3gdcimjsj.html


<!-- 参考信息 -->