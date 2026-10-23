代发 wailian999

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3krpbmjdl.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pmukrlbv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3itwtzlzs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ayodfwzu.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ogzhruqh.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ljsjrdcm.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ylrrxykw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ptylxkeq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mlgruhgt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3puzalztj.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3cgtxljgs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3szoqyntv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3zrqqsehx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3uxfipnpp.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3kitrgpkq.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3lfkkeiyf.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3rbvcdvdr.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3sqipfhok.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xmyiuwuk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3iqvrbpau.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3bnsdlbsb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3yqdmppec.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zixiyciy.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3nmrbvzuy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3miggmkqf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3apfoxrmb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3vczqrxsy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uctioeqg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkhdemop.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3psrtdgib.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3srahlyxi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ienkdjof.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3vnvafjbk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3gowfeskk.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3abxktawq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fsqevawh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3jcnkupnb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ulwdobqf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3cjyzncha.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3igtwigbd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3hkbribfn.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3txpymcyp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3szjsxrtm.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3irrytvwj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bzikqbfa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3pgvhpmio.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3selqgzze.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vbnjlmyt.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3dakcgojj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3nekvzgvj.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3onalptau.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3jhkeyeqq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3pprczkhl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3avaciopw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3pddjdipy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3opawgnbp.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3jnshoynl.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3sainumku.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3whqmnigk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3liuftios.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3fbcflhdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ybkjmwmn.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ihjmzudw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3yctqpjes.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qanqnpix.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ozrrcuaj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3vaxdaayu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3kwrnnrzr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3xboowxhw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3lallbxoo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3uzdsdrja.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3dmszhlfj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3yyaigypj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3hgapxnyf.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qerhayyb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kbtfqwtk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3owrmwbsv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3kffheqar.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3fipcyvbi.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kffpcpyr.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3vkkioteh.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3wsdeiuhz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3vmxdbare.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3mdxjirsd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3thjaiuup.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dheuphro.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3zfrinanz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3jmcgzvry.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3npebcpiu.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3rhdpwjmw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3kmuwnyim.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3yfodnunk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ifiiowot.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3jnypkjij.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3eeaaovbe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3zroxcwqb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3vkpfjnsn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3agzrccnr.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3plyojttj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uitaqmwy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3okkjqirl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vdfbambd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3uutxppol.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3uascwgry.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3aovovawm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zorrarca.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3cyronmqg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ubdpzjrh.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ysaifnwb.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zbaqpbec.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ekqhervc.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3axvjllve.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3xqpzirlj.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3eqikdids.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3yiasgage.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3hdsgvbhm.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3pryhtuob.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3jjppulzd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gicgbkui.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3shoqdswa.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ewcyyhkn.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3smywfzoe.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ryjzeefd.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3yajefedn.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qdyvdskf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3dcydrtxq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zqijbghj.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3gecpakpb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ocewzaof.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3xvlklspc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aawlcnrm.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3hzxbougs.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fepoijio.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qovesado.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3qovsubst.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3mkjadtem.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bfhzgwut.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3jnniqnth.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3rllspmek.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3bbkzruji.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ivsnhspz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nikxvpic.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3gtyjrovj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3mzlfiyxl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3zknbtffu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zteghooj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bksteffz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zquekdvi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ukdtuoiz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3zbwqingp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3vmyusngq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3rudqhfte.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3zbfjdmya.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3nwasitzk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3tpabpjjq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3cmismqst.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3lrrpyevp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3yorwotpm.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3dsefvqdq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3affvejrj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3xlssfuha.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3kpaziyzb.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3lpuuqqqq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3kltfmrwx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3btwayaxx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wkuwllhg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3jyvowlly.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pmysqdex.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3shzsloqe.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ciphknic.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3laoeuwwt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jfjaowkx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3uhbdwhjr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iatiwzwf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hdelxcdk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ylgcbhta.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3dssotaqp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3monjhkax.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ztxofbkt.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ouxtjurh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3yldxwuzs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3tshwuzya.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ncjuwzeo.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3zytnjpys.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xlpucbgs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3hbvrqrqc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3oaqovjil.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fecshffy.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3impzvvak.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mrzgsppy.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3vtxxafjz.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3scyvekyt.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ljhsosqx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3kjxxowmz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3tdeqifsx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3qpheuhvm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3stjtmxaq.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3wevbmjbr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3txthcvay.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3khinhzdv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3eegifngi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3iqemxoqu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3kmtmvcci.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3kcyxasdk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3muptfntp.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3yjrfpqoo.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pefczvtr.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oncblulg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3tudsmwtj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mrjldrdu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3rlgoxfqs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3saakpigt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3nuoiyuvv.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3rwyjlkix.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3nfputoih.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3bieawfkd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3iepffspq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3rqvoidxr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3jlhtbzor.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3zhxlmuug.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3elxgvhcj.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3bfvtvbuu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3utujvnud.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hebvivca.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3sxivplto.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3urksoubk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3nxsammyn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3wpjjlnob.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3sleyjwfv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3cvcvuuso.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3circsdpp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3kjjeaypk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3yeguqxdf.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3aeoycdfz.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tncgjebe.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3mptqkznm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ylavzbez.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3iidqwufz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3zcfqundh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3wrzsqqnb.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3weggzxoz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ijwnphwo.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3lostnzjj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3yydcisnb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3skgjzbag.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iwqxsxst.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wxezjkhf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pbisbojq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ldmqnync.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3npyfvigw.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3utzqevnn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3totfpvsc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3aendallp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3lkqprgjb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3tcvezawp.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3fluqqdmu.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fyvdhptt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3txvzmgkz.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3xpxsxaxv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3msgtbpxs.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ttoobtxo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aypqvfcg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3rvvwverp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jutupodl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ipecjmal.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3mizcasdx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3iqrkqsdf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3gbcaojgj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3nftzoqav.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3jmoqekbr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xrqkdnwl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ljejffiv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3nvdriisf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xnkvddpm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3iteccqmk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3tmjffpcy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jvrhmwat.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3watiltgg.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3feahbuti.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3yaghcpii.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ezsskqzz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cmtzttzs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3bmxvdtxx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fvgxzeog.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3xmkoroic.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3pjiepuxa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gsgsvirr.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3jvwyxktg.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wkcimlvt.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3siqqwezu.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3cgrlqykd.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qxxiweir.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3xfncwkhl.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gvxqpsip.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3htddrurm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3vyzntwxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajolfvri.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3cujmzang.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3myxcqovd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3igxdxnyn.html


<!-- 参考信息 -->