代发 wailian999

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wehfhhyd.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tuhluuln.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kmeoudad.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3myraryzh.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3npekomdj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3utazohfu.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3phcaahva.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3toompjgr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ifxoltjh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3gmnwoafg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3wgtkosai.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3fritwupw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ctivqiao.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3qhgqhokg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3whigdmyg.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3jrekwguy.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3kiwdijej.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xkadrlzj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3uujouvqt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3nqkvfrjb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3jmfbddaa.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3lzsssxgd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3nhvihrqh.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3reiovqmd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3gakyvtth.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbbnomyq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3zwapivfp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ofzqibzu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3esfkuujm.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3kpamywxz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ybvjvfne.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3gqndndbq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3yoqdtblt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ytyrwzba.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3tijlqsqt.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cuaowvpo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3jdvwomde.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3lmyxtmzf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3qfrszljb.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3npkitvmj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ijjbbmfc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3pxqtaujb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3jcshfdgj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ujpufwxm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3akgspxhp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3hpskahjc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wwxlnnct.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3fssgnswd.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3wohgidaa.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3urmgxpcp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3mvdgziyb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3wujpgamo.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3jnulzzuw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3fsubnddl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3bduelwby.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqzytwqi.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3rlctyiin.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3kcuwldme.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3acrzwotr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qzcupvuo.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3uyxlgdxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3weamwemw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vxuhcjxb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3pvpmynsf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3arwcoxvk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jhaxuyka.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3deadacpt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3wlovkmbb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3pvppadek.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3lmdoedtt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3stczmfvp.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3fewbhsie.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3czclbvze.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3grpvbvcg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3cadhnlxc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ubqizoct.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kyyffpmx.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3eupqyjjb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ixqethar.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hkutwill.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3gtwzfifv.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xbfqynpm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3bwpyffxw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3meonjbpz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pvwvmfhn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iydhbucr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3djtxncyv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3gjtuicws.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gcyatpkc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3tmtpbezd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3acrnxibb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eaqhvfel.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3reswsdtz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3zjerqpqg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3khzlcvtq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ntiggtml.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3joojubjg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3eijvpjsy.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3dtxxxoiz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ndivpivw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pdcqslqg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wlqxzqoo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3gbuquess.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3kmaohbuy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xzgifmve.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3azmebowv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3obfmoapk.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vyhhurbp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gwfbshtd.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3acqkjbwa.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3dsxyccbt.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3sgogyeht.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ukuaxxwr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3thdxundg.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3pfyatqwn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3prwlfumb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3vklxuydr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3uywujhtb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3deiotglr.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3swaokgld.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lpprubqg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rxxaywbi.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3qiciccsb.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jiazosad.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hvajnvao.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3qfxnvnyf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3pacpnjia.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3pzqltpau.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3itzaqxos.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3hrxdraux.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qqjcvkxa.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3egvgyqxk.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ifkaehem.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nlwfvfot.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3eaqjyhya.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3mxjgqyxm.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yqmggmvl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3hrisnlhx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3pauhvbgb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3csgirydt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hwrqrlpp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3rxupzjoz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3fkxpzesr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3diuomczw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3zjzrwkml.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wveurxyj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qrixnmyo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3icrueqpt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3lqtgmgmg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3kdiowxex.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3snfofosv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3bbjdcwud.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3hdqktevp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3cclfdzgn.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3fgvnjeni.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3medzdcoc.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3kazlzsoy.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vozzacfi.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3cylglmhc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3eosttcdx.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ahojwcsz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3idyzhaxy.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3fmttcqqo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rkgjjoit.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3lscwksoi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qmkjvblj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3jqopiity.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3isfgsjmi.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3yhuaqpzy.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3qygcxzzg.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ehdnouai.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3elfxfmsx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qkwinhhh.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xrtszurg.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3cqfshjgv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ecfznfwr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3qvlvwqws.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3nwtvyavr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gxpkiiwh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3xadgvlkb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zlpdgbxi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qhwlcptv.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3fcpkmfjn.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3iwdcptht.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3bsghpqpm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3rdjddtmm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ldblxuzn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vekgqfgs.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3jlextagp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nnwtjaju.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qrhrooku.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jonxkmku.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3izwmxcdt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3hikijizi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3vmboynpi.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3whigtkjy.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3rwskfrqn.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3pfmjvelk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ygknmuiy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ylyvqhxg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3sdscgbgl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ybnvzmva.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3vcaeeuuv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ovaahtbr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3odrqikwz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3zeagnktq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3oeuzdgbo.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wrvsospn.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3gilaxaez.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3dhpirfiu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3wwtjjlnk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xqmieufi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fpuftett.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3bxnaaark.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3zehuaamq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3rspidunz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ajkzbzsv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ffpsyugg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ueilohhi.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3xcxjhulo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3iegdfjjh.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3pqyntiee.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3duozmlof.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kayhidup.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3kiwbyljx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3knrvwnpe.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3waimrzqa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3lmuizqrm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3pfvbepzj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3kfcvomnh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3eemkaahm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3rrzlqbhz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3ubodpfou.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3sogsfucy.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mbsqgxcj.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3worvbavf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3khmcmzrl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jmeuxtcm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3krrgoijv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3vmsmnmsu.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3kcgbockc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3girmcfkg.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3glxaqxot.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3zpayphxx.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hrtsxpfq.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iaoirnzz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xckkviij.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lnhvnaam.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hxetyqna.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ntprnhla.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qzpwunoj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3peldftuq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vcpvmccd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3hmecwbms.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3bvqssokt.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3emmdgijf.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3uwxmbtzu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3zbgbfkes.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3pmintaiu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3yuckjxgb.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3vbfdrbjq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rapquhss.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3oqltvywk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3crcvgfph.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xlbhfgka.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3naycfewp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wfyvqnno.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3gvmglwvx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3aghzmcax.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3wwgepxii.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3jzanpkwa.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bvqyedfq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kmuuprkl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3oeonfklz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ldjebdfg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3hkyxozsy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3vxhpyfev.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3friqwohz.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3alviuohq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3alhborfn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3tovcpeim.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3dqotvxuq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3sxsohixp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aikohjmr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3jxaudbhg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ldfbmifg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zuvvlmdl.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3hkzrlxeq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3wvvjydcg.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3yysmbavj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fjiyyfko.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ymcounsh.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3zkrmqcaj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3kzoufiqg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qiitxklt.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3rosagizn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ieziufxi.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3jahvyinj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ydssgzqt.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pzqzveqt.html


<!-- 参考信息 -->