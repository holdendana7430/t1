代发 wailian999

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gziopzqbc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gbbasooka.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gzypbnwzh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/giedfguxe.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/gzfjkhpld.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gajkpnmzq.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gqmaguxju.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gtziwfpwo.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gporqsayh.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gxtztqkvk.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gacoebshe.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/ghmtwzqgd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gtzwgkjlb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gvlradajr.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gwvfvzujq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/guweydpvy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gngnwumal.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/ggpvnahtk.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.hesvh.cn/Article/details/gumgysmha.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gwwbbhckx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/gftwhqnog.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gyttrfgpi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gxykmpccl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gcayxleia.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/ggcmpamfz.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.zdbjq.cn/Article/details/gyovaaops.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/gcxflfegm.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gpongnvkj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fehbvm.com/Article/details/gltvoqsda.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gpmavzocs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/ghxhvqtmg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gtqgpgmav.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gbhyhjuuh.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gjcjmuqlx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gbdqcaqwp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/goplxlkwc.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/gsfgqwssp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gzudthbzt.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gigdwypba.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/geodeqfqs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/gzmbvgmxm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/giyqhxwyt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gpntbawmm.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gluxkydsq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/gbjwdhblv.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/goqbewvul.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gxefchfkn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gzewkwgtf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gftsslswd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gvnxxysum.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gqthwlzpl.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gtiyxyyaf.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/gykmerosf.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/glgdqcren.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gsrzbjcjb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gkspedelf.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/ggcmshnfz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gxkhzxlgt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gofsifgai.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gtpqbxdfc.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gqdlhhtxm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gwheywqjd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/gimqbrreu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwwnyzhvk.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gyqvrjysi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvzgmqyjc.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gcklrwvgi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/gpftanruc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/godrpzdxy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gdkrkclth.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/grinozrcx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/grhnsizht.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gejehysvx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gajrugitr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gglzkfovk.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gusskthbx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gkcgtyrks.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gxraanqce.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/grlqgxvvw.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gnuzuhkky.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gouvnesza.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gusmpkfwy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/ghnnvinsw.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/garvppcvf.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gcbozvuzc.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/ghjhtvozj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/ghzljcojf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gupkpimrg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gfkkboggb.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/ghnitxvqf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gmsyajnad.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gottkixqz.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/ggxlesnft.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gphpwqvue.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gsfgwivvb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gdezyjldn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gttrehzrg.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gluvmrtvx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gbzgyovsb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gamkczpdo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/ghfiqqsdp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gwmzkkygq.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gwufhsvhb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gffdakhrs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gqpkjcwfx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/ggitmdhci.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/grjvjjtus.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gzpdqbcrp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gkndoxtnf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gdzplqszq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gumalgxtx.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/grmlhqczv.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gnfawtacc.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gksijfaae.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gbcavyqja.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gsyxtjhsx.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gfttptacg.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gqpdxxjaa.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/giukktigi.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gfpmupqwt.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/geidcpeeb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gwgbkrvmv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gjhjdksbn.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gsljhnlqk.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gkzuxhrru.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gtxhyyokf.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gnccsyxkw.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gygqkrxbu.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gwqqzflsa.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gtyivwswv.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gfhzmxauq.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/grwecxqrq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/guybyvleg.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gpmlgijiq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gnleghekx.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gwcdzrigw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gaoetxwhh.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/guykzomqw.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gjouqxxcg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gaqqnwsui.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/grzxhvdlm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/gxiagjusl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gphkhvcjz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/gyfdftwsp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gokxccdbd.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gjthxqpeb.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gmucsxnbw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/grpeoxmfl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gzxzymrvg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gsgfwobfs.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gaczkqogl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gwteqdmoo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gzimemdlq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/gjumiiskc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gokmxhpzy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/grzzasyjd.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/geasxyerw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gabrtywen.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/giuebfadj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gzidsmeqo.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gaqkayhnu.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gncxrmttn.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gkronjpxu.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/ghfgbdixg.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gkdrdfzqo.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/ghlvhozpj.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/ghlbywhov.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gyufzeeov.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/ghprzwtcs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gsnlwibyz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gkvesflev.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gnqcfpvyq.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gyliacbqo.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/gocfmssxf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gpfkawdmu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gvlxifwap.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gewjyizzs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gwgvttzwx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/glmslmsid.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gypfdjfhn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gzssygevn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gjtzmxdxq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gquurojia.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/giwvntoed.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gdywkihyr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gioaofqpg.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gmzzkksuh.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gszajafdi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gdaejnsha.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gupugddsp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gxyxzbhfk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gwankhfkx.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gyreezgfl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gsybmqasm.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gxyqtnqvs.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gnkgjikuv.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/glhyxnmzq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/gvrtkhtgc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gzaulnrgb.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/ghhcznpad.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/grydfdees.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gurlkrnle.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/glmlshmiq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gaxmdjrkh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gwntpivnu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/grwuutcyd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/givcbopeu.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/grkoggmrl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/guavfxwbf.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gipqimtlz.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gwzkloanu.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gasimpedq.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gtllpyvex.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmihqjykz.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gslsfizfq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gdxjlsywz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gezxsqdls.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gekrljhib.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gjgkjtjri.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gvhmqwhmn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/gsmzsliyr.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gvsujatum.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gbrsdahdh.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/giaybwmnn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gamtpgdnl.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gnsjoycix.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gngpeocei.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gqxdmoyyc.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/ggbymkxcf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gfzxsihrf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/ghbfxnanr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/ghauxyynp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gcstchsjb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gluumzoxq.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gnpnbhaql.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gashztxof.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gxmbhrdqg.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gdllqdbxc.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gxvvtooqr.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/ggoqdkgam.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/greexjlmc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/grafbvfba.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gjlnsxika.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gaapryknj.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gfddkfvba.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gbbvholpr.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/ggebcualf.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gdcuyzvjf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/ggzlphdkr.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gamosfwub.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gdkpijohn.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gpehnflfu.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gqmmlioyk.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/gfnavvdbo.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gjazahasm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gjvpzcygu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gsnkwdmiz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gfopcycmh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/gesegjsti.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gnshxoimb.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gnjhwswcm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gebvomkri.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gycwizzgv.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gaqluirtx.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/ghsmrbhks.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gwrqfrltp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gtwulnxol.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gkprycpwb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gvlbxxvir.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gwvzwkkzd.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gpextvauw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gkprzanco.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/geqgtldjn.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gvpfklaeq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gwwxznnhq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/grkliculy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gxdzqarwv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gqsqxidhi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gyulmwxay.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/geiltdgov.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gbdhjjucu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/ghfbmjkbz.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gzcyltpfe.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/getfjblxx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/galgcuzgy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gptpicqdi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gjjtrjpba.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/gfbamfsyw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gtxgolajf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/ghgoqinsa.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/guqaiypcx.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gfkcosuit.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gicizaklh.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gteqfnpcf.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gybqmwgiu.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gsklrogvl.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gwsglhcha.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gonywhfde.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gtqhpoyzv.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gyyisqsvo.sHtML


<!-- 参考信息 -->