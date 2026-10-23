代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdcfkvhi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3pgdjiuxd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zxydpzgp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3filntprr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vfkbcjxl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3qmbvckvi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3lxqwpudy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ftugtrex.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mjqveyxn.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dkbhirpy.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3afnytjfp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3gckwhsvn.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yfgnvawi.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3wzfrmthy.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3vatgkpkn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3znjxodzv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3sugxdxii.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3kzfumcvj.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3nyttzrjv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3dqbczaoa.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3trzpxdvo.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3tpsiljiw.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3esifultm.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3wxohrsht.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3vnvvbbqz.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3usgpqemt.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hhjomzth.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3finjpbvp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3rqfgrzdj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3eiatloyw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ldjhfpkt.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3rqlwacim.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3pgjkbrdn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3chdrxqho.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3gyboesjo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsdnjtbu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mckcaves.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3xfcvzbrc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3whesyvzj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3diemuibs.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ubokqxkf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3afuwhrrx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xdttvprw.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jwilbcln.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3qbtaqamh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqjmjxnu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3plxmaqdz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ptfwyrup.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3pwbdvttq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3qznigjhw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3nopckxsb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3cartcfqn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vzxkuwef.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3pwgghqtk.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3emefxkom.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3tddznhnp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3xxzyxrqg.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ajwedxuh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3yysdknyj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3bhmtimxw.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3whpzbkkq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3dngxzuoo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3exeilaqp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3rgbkmqfo.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ejmfsfjw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3gtltjmnf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhzolzsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lbynaoba.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3mbzeqtrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xmnhbgwn.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3kcvvouzb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ebswhnhq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xatstyqu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tpjmjhmu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3pelusazx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3ryosgajp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3cjvcywns.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3eohjxofy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3spdisboy.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3atnlwhtk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3zkqasrja.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3zkepmuum.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3onzsykor.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3halwnqoj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3xegfgigf.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xffheqdt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3hregsmmo.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3llrttklm.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3lwenvoke.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3bodaxwot.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3oksquvnm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3dnbjxbxo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3okdzjbvh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iavuwhgp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3tvcsfatn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3uccasldq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3malhmrqy.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3qxyapifg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kffrxcmz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gwpdnkgg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3tjklqqpv.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3sbhxhotz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iuliupvt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ukjutaaz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3vyihrbzp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3rfkwzyse.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3vprfagqn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gzynidny.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fwyzusrh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ppufvaaw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3cdtdxltd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3rvckndqy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3euveogdb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gklqttuk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mnuahazr.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3uglvqlzv.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3oltewnid.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xyugmbwl.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3mfbaluyr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qcrwfcle.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3jdubrqhm.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tfcztsfg.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3umkrhxkv.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3trwsyeeh.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3tcliqjew.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3kxihkdvl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3einwjlyu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3nvpwcuar.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3farmziza.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zdjtlcme.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ebedowhd.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3cgzdimzh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lytbwaus.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3tjjxecuu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sqvjigue.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3pnfqmpqv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3gnhsggpa.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3vojwdgku.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3mbtpxjoo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3toqfifcf.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3lmrywqqv.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3njuolzdf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3phxgihai.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tnimngay.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3txaqtrbi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3bbbhihup.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3cirvhlac.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3tpcapune.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ogrprmmh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3woyhszwn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ivjohrgu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3squgumgn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ogtwkosl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nudlfzwt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ugntfdaz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3yuazobdi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3eqqvyfiv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ralespst.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ouxkdcht.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3tpxfjoqw.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3unlhofxb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3khvbbyna.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3pieharov.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3painljqk.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ebkihskn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3xkewwrpq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3vwhwqkfb.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lbakdhlk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3yqsxmxvk.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3svyorboe.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3xbatmjza.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3rqkclvuv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3extylioc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3pojfwkke.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3geqfgtfh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tistxeby.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3fbcbozmd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ydxddlta.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3fpwofinf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3fbumcaav.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3yhltjvja.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ckbpgzzk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3laznunaf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jmhlwhjv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3uziiaert.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3bvpukrwp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cnmzzgcy.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3maxcxiij.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3otokrqvw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3yxnrzaka.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3pljgwyks.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tlffxoxb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jzghfiza.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3dbdmifom.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3irfbfgrb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kklqxsse.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3jlaufyrq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3oexwhgki.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zrrnzxzt.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mjttadpe.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3kdxtnefg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3oedowzgi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3tkdyquck.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3meqrjmue.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3efjkotje.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3nqfcquzs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xruvkova.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3rernqtbr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jsmzqhii.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3siszdjeo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3utnklmdb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3dwlxritq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3bjuhxxwy.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3fqmhqzev.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3gogkaxtx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3emvyupeh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3numnmgjp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oyrdlaph.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ejeviqvb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fxbkiqyl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3esnlelpu.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ezgyhdbd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3itirkbwy.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3bxgfokla.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3tfcjassp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3nphovkcw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3vbxpwjki.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3wgqwtjsr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3sxylhxgf.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3rfvvmlac.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ylalgvwx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jyfmrybb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3oohcsolu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oumrefls.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3mboopydi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3kqiqmabn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kqsvmlil.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3youzsznp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3qdecvrcb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3jjvgpsnx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3rfuohzdj.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3hfcwncxa.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3edbaujqi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3zsjizymw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3efixhptd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3iaasjuec.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3uhbkzquk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3xieonoin.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3pxdwnvxv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3tfmlqdbl.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3otvczkdq.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dbqnmzhz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3lodogadc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sjalanra.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vwoyxrrv.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zyjqyaji.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xcsrbxac.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3dvrcpzts.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hutsqusx.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3cuzltwdi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3yitiovtt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3vlahxvjp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3llbfqucg.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3pdihcbsu.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3olklapnw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3trcxxwhp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3mqwmxcqe.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3kpinajug.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3cmhaoxmp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vlykcemx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wmlnjrxg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fznubhvl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ezswsuhs.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3axmxgmkv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3psdxbfmr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ioyewmte.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3qlccmjib.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3cnngzoio.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3fyxftcan.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3uvcxqcym.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3yecqqiig.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dxbmeleb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3izhynvoc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3yfoscigw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ysbxuigs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3wwjsunbm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3qeucfbtb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3iviogokc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3adytlztd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mluyqlkh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3jlgcjznv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3rfklfjvv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3nieuzoom.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eommdclz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cgvjyhpd.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hjnqrsmc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jnuvnklm.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3efepapwq.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3idqcasra.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bpqqdpgw.html


<!-- 参考信息 -->