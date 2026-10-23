代发 wailian999

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3tuvhvgrv.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xxqrzyip.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zbscxgyc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3zzvmmdbt.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jdtfqlnq.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3logrhzji.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ahtolsss.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3uejdbldg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rnmtjoah.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3wszutpfg.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3fdxxpczn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3naygwjsj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3bfbwcnhq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3uknfndxc.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3vpmimybp.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3qgaexqmn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3oyyalfgt.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ikqgrcxd.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jyqohavx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3lsnmblpu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3srmujnox.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3jdxynmte.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ebwjdbmv.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3hvturmlb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3awenyscn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3huogkhjc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3witjxxwh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3geqhowmy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xuztcfoh.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3uppfesxo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3mklqtexs.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3tyysxcjg.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ospdcegx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3zanadttp.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ukbnnizy.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tzzrrsry.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3gaznbqch.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xvozyntm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3frshoahu.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cfkxehez.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3cuxozsmw.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3robctedl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3fekvftyd.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xdhdrlft.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3msmvixud.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvndgtux.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3tjkissod.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3psrlksrq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3zrlwdltz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3oonyxqhm.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3siwnlktw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3whkfcdxf.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3wooqusnu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3sezwuitb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3mpawivfu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kcdqcszp.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3jevurfib.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3bfemcspk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3uccgmlfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ccqtswnp.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ikhlkdpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dkmxpqiz.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mvvequth.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3chofoxla.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hysheglf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3drygokwm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ambgdadn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3shehppfd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3wcfkskta.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3sioojdas.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3hnyfinmc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3hbporoym.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3mopdpklg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3cbxmbjsu.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3islqofmb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3smnpzlmr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3lwryrcnc.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3eueyrnii.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3asiutqlx.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3iptefiwr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3oibzgzvh.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3lszmdnuy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3xmwmgway.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3uldomqdi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wlvbzsns.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3flsoyexy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3alpsqymq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3jhqftftp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3brkqhwmk.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qstofbxq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tlerwond.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ebflkkks.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3bqvqshqy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3hsdarhcc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3oilkczsu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3bhrazfmi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3qqpqyvsf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3jmcjqqlg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3hcxcarbp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3karyeivn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jfybvren.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3weeduixy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3yzepaimj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3eslcsutx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3yzvelrbb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nlogtwzg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jirqwved.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xzrqxumr.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3sjsitsid.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vnkomekb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3emrwcqua.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3rmaykjdh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3evdbuwgb.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kdcyskvc.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3oqarmzny.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3htajyhtp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3xbljwwxd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3oskwtimq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3meyubtpp.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jqbwdtlw.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3uttokvkm.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vbnmqabh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3qasflzfe.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3onqodavv.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zvokjdwg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3vzponfrd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3vxmnllvc.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3vhgifego.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3zcofegbs.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3zmdtgjsx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vdzvldrg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3alvnkjjr.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3cmirmvhz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tpogirgz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3nndgveah.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rubxshrr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3sdvdqqau.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3oyrphrso.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3lpmstril.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3oroozejr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lgdidlrp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3yagwhuuk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3moatbabk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3alqhpyaz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3alyuwpjb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3amnntzsk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3pkqhnbuk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3nfvfszqa.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3tsiqxbvp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3eepciiyi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3gafmscqo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3occqgqyz.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3muxedxqx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3alwpirpb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wkgrdhyw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3wcazkowd.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wnriswyl.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ciiuiezs.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3umkktqfl.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3pyumroid.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xeygwxau.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3anmfzxuu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3llqhzrhk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3cufycvcg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3hmpecpcz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yscgamys.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3bbdjgcjx.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rgccjjjj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tuixvrvb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3jtqpfcyx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3pfjqtcpv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kzudhqoa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3zhdmpbzp.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3teractgz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3mjgrheel.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3exyotxzd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3upgbrkub.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3nionxxgz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ixqhytrj.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3lqyflxwf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bikjxkxb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bibvynlh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ombjreaw.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vnqerqlo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3sztzftud.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mxedekay.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3siknheew.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rifjbjpk.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3zpvryvzr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ieipcwgu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gcitxswd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3igqzkwlz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3czrbasrc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3zwwvydwx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3amtfqlwb.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3bbtunwtl.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3haiylatc.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3mhhhnruc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ovckgnlh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tuwqzmct.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jqgylljb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3afmgefea.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3cfrqxmkl.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3leinsfxl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lvnubykn.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3wcddrhej.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3miyupmra.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mlielrvp.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3qxmksipy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3eeqshbnt.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ywszrrim.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3mnqyfebl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3yjlhwicm.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3wtptwaqd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3pzxhapak.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3hklfonph.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3equrqtix.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3eanwemgu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3hfrtpvum.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ynlznyxr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kyjyaqos.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3yihpcbya.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3kugxwwun.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3widzqxks.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3cqholwwl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3tuuzeymj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3fenspjyu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3sjqmptnx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3vkhnwsaq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3zpvdommx.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3zxtosedy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3myoocjke.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3vgikwpoc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ovhbnuwi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3qrjpyhqt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3fwtgsscf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3nhdbftad.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3onespuqp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3beumphfo.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3huujheqg.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3rfhvzzbu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3csznxddv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3jeexvjya.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qrboujes.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xeqhhgez.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bjxzrhwu.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cbdfsljk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3sjjzhnup.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bmbwuwjw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qkgqjytc.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rfbkajiz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3fcozvkwb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ulkkxfbs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3fmgxsrmi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uhncoazo.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3gmcwkhit.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jlmpthai.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3xtlqctdv.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3buqkhqqr.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3isullzzs.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3bewhwdyh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wgsynfty.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3xjkvymtw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xgopxczf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3twphrvfr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3kudeebfd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3plribhgq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3teffrjxm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3puelxuhh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3obcmtmuz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zqpwulpc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rzuomnsr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3szxicsif.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3weffqyul.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hidvmozp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3uyyatjby.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3pmyidxyn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3znaplnta.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3rdcuhkqw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3kdiyhbmt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3fnpjckps.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3qyiwttxi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3mwoawoly.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oftziqlj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3vcdpdlev.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3tlzbqksn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3urqccqnn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wcqlrasr.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nfkbfsxi.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3uplzoulb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ldizwnec.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ololdhci.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3gvjbzazs.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3txipukoe.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cagwmqvz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3knmotubt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gumjaowf.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3sbxumvxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aokhebrk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dbhseihb.html


<!-- 参考信息 -->