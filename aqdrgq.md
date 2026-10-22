代发 wailian999

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2hmubyril.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hldczooz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2icxigtzv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2kkgfmyhk.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dsxzmyyc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2nbkbuhhz.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2titlykog.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2wbgirubg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2cywnjbzm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2vdrdvznt.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2hrsxcskj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2wvawytgn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2iglcafqh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2setpqhnl.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2vkkojvcx.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2bkyxntyu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2usgdzvgj.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2osrlijgv.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2aokgvyeh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2fmyqctez.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2sdvclkqo.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2uqjnvlvm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2wctemxhx.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2nublvlgh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2olccawts.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ueonpvlv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2kbeuhlge.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lelzcone.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2njitqwdl.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ycnpqaba.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2iaghbhtv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2brzaxtyj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2gjsmudqg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2cftvhdsb.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dupywbxa.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hulcfqgq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2exywmmcn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2mgpjrzey.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2qdxhbocl.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kdpbymvc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2xhcbtrcx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2csnxwsfn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2vqtgigal.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2tavdmuax.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2xllidcre.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhlbgizn.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hbflruka.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hanccvql.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2sdbbfozm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2vggwdtys.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2yioelalh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hifxkypg.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2yhtdoxgl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2dltmhcaw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2gtequfno.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2rnyhfhaw.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2iilmlcvp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ypsftzug.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ggjlldyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ukbahcqd.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2rqxevasc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xpqwfhfl.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2nxcugamb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2lxnjkkga.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2pspdwzsz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2witxuklw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2mmxscaec.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2iulvnral.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2qxcnxkkg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2xqnpnxqu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2zkslnigw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2basmooty.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2umrivzpn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2anljvwuv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ebjzskyj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ddpxlvhj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2dmcpbtcn.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2hpmiuljk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2uudopoqp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2weugqjyf.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2llpjjpwo.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ymwexipm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ugmstimn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2dqqlgtoz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2htzuwizf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hwlxtskm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wwhggdhl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2cgzszjkk.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bzyzfset.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2yjvbvdlq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zmpsmzua.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ychxcxzg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2umqnlrel.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2paotcohz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ormqzvso.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2odtzwwjb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lnilgini.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2gpghtqcl.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2haziagns.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bslpswsa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ufwektln.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xtgdyuse.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ypwkrjgn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2mlcmidmw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lltpizpl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gmsqmwes.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gybroytj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2nhmydvfi.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hmukajwa.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vduwwust.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cufgsfvf.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2xmdsqslv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2fbxxusbu.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xzrgtufh.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2omgbownk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2dudewvth.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ykdcmqpg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2wtiaykls.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2chbqzwgz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rndkbzpk.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mmrdulxf.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2sqbhgayh.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2qgvxsfdm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2irbaidze.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xgerzkot.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2tmqnzdaw.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2cfgmixns.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2bshaybhk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2oupjvikn.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2rvfkcrvo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ckbzrcld.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2vtvbycte.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gujvpski.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qshrxhgd.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2sgvyiywp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rpgbmewm.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uzjuehdu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2cqehwotk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2lixgjbsv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2orsvtxis.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rezqonrt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2olbouuos.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2fgloprrr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2jskjmhpb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cxueveig.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tdevllly.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2bbuekbtq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wdbgxxri.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2mnhwaqkc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2rtnyftqy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2wmousoxw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2qgseplgu.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2mnqvrhqp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2uxvsklzs.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2emnpxneb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2bknjmbgm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2qzlyhiwk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uidwvltf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ewteevmw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2jpwtvnfa.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2zofahvhh.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2vljpfzxv.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2vcyrytzy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2zgtywouo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zfrbkwxy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vlwljbil.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2yneruzev.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ndpbuybz.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2rugxnrox.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2byfmaqtu.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2qgwnzdyt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2lowykedi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2gprxheot.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hmqxtuoa.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cpalqtqm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2fkojlsmf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2brgfygdh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2igkohiox.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cohnqtyx.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2vpekehmc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2iicznqam.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2caloedwm.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2muxgvcan.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tmergvpq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2khjbbibd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ohsvkdkb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xkmzygvg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xvfoasjn.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ikaksdiu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fcswnllj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bviyebpo.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tainlqfp.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2gaslismc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2wmtvfsgm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2kifrntdw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2zzlqkmfz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2kvypocdm.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2gkfdvffh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rntsnkut.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ushhcuuh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ezgbdzkg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cgfmojma.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2esqhqjyp.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2xdbdlsbj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2uctyhnyq.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2gthzfbhi.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vonjjfkr.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2hxtamntl.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2lqyhluqm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fhqhjkci.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2btgsvtxw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2dpqosnsz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fongoxmo.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2kbseudln.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2pwxkjaeb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ncqjkybk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2thjreenv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2adosemnz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2oxtnwnbs.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2hvjsktqf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2hhrzvvjg.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2clmaoqfr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2lufrahhb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jvrfyvmc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2atczpjeb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2asprqctn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2fjwazlea.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2iqyvxpij.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2gfkuvrla.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2tajtsodi.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2amsmktqk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2nypmptew.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2toyuhjpc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2yiasjbgs.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2qqqpuwza.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sddrjfam.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2xtkepbcn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2upnbomoi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2cgehbbwl.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ehoshbiw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ezrzbuhm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2pycfrvfw.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ttsyiawx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ljpbvbln.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2rwbucpjy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cdrqgtbm.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qcwijuvo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nkbeavbz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sydprfws.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2rzigwpdu.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ediunbsq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2iqunpjjh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ncyzqhlt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2qsgsgjgq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2hffmyvnn.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2lzjlsheh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2baolvqwj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2hjllxifa.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2grzjshyd.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2iyejjcoa.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2rgkxfvvf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2fdaodgej.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jgatycdi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2cbylvwza.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ixfuvlhb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2fqoggbfp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2hozgkfcg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2pdpfddmb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2luszmygz.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2crtxyupb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2lxlxxkiw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2xaifixss.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ievihzub.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zaqixupr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ayhyjwzm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2zyzjzscw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hcznbkwk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2tcgnmzfo.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2wxbnprmu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2gepxlhcx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2flazpbfg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tcxoxnml.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2modologj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yvyutfee.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ydfyojtt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2jsypjxgr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2osrdjmqu.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ueagigjt.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2cjncvwua.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fxranmyn.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hxkjmods.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qjlhopxk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2sybqkgfu.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2lldkyles.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xxpauaea.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2kexxdfno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2akzydecf.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2akuobrls.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2efnmfmee.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tjfswfyp.html


<!-- 参考信息 -->