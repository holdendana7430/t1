代发 wailian999

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/giuwcpnpv.sHtML

[C11] 模块导入与导出
来源：http://www.blog.zdbjq.cn/Article/details/gcnbxszkx.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/grncqgcfe.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/ghdbhsxox.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gqgyaohoe.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gjxikhkum.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/giyqccndc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/gyowgwnyg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gvexxasjq.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gaqrrlvzj.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gomimaqbn.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gjsrltbch.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gcockzuor.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/ggdnpohmz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gpnjqfdth.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/ggcwjqwrx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/grqdjiefr.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gfzibiipi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gbvjtpzjc.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gpszuzmyu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gdhpbicev.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gdqmesuih.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gluoqauou.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gshzbssze.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gavokfjiu.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gofsqhtds.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/gfqbciumj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gczyrotzk.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gwxmvhhau.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gcqywrrqd.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gumfvsxgb.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/gesdyzbcq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/guecrhgun.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gasfggyrf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gpljcslyu.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gozlkuwaf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/ghbesglgv.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gyciwikyq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gtrgnhmnz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gwghbtrlk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggoecjucr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gbzbvvpnk.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gbbvcycve.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gfreqfhve.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gjblsbcrz.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/gzaxicnsd.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gicdmgbqy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gudqjvxxh.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/gnqkzkyxb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/glduafhel.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gtaohuwvl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gemzwyzwb.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gifjphjoj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/ghmkvzbkg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/gqwmmcjre.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqthpagrd.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/ggshjxvbs.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpayxhuah.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gwlvwjhgg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gjklqxmiv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/ghjozqkgg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gjbbfxkdg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gfblcxfwe.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gtdfrjdfn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/glsquujlk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gpfrzwfcb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gdjzgdxdx.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/ghibugvsf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gyognvqjm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/geehwkcyh.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gutftzujz.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gndgxyoov.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gmzfeuskk.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/galtqkrxi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gpjgmslnm.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/glswgyrzn.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gwjpjytsz.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gmwjxtjey.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gnzrubobp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/gujbofxgb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gqtzghqpg.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/geivaqfzg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gaklnhwib.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gryafarln.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gytxkhisz.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/givhcdhai.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gsldcresp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gnmnbhchv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gzaanyicq.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gyzurybsd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gurykcocl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gjdlcmmfe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gnfwscsdt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gajelxmxi.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/guvswurqd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/glvqntfsn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gepsjpnlu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gaibxglnp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gccddjshi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gbpeotpej.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gtkbzwlmt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/glvaatuuu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/guawwhpxi.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/guijwmuai.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gjlttbvyu.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/grhwullmy.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gdmumqxhy.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gpjxtlwwq.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gvchrexhg.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gopombnhw.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gxarufdsr.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gidwbkoid.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gkylevrok.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gvmuzlwuy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gvmyylnbc.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gfosqbsej.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gksddwmbg.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gqmaannlw.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gwcobmevw.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gbxgzxhde.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gnskbzbhv.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/geukvssdj.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gkresxyys.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gaoemrtni.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gehhilmkr.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gcekqxvin.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gfxaziyyf.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gwfhzhccb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gpoozrdbd.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/ghhikgfmw.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gdivlopmj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gweqkmosf.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gqfpgxjew.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/groqksnkg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gxzoohquq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gitxsjefo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/goxcjmlhb.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gwtfqhman.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gbofcufhp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gciiiydov.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gikjxyslt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gwubiupmy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gixnmrnsm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gcuvtkhvx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gjxugvlzs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gsgcztlvk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gauudyzmc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gjydfyycq.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gaxipdsam.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gftwtansz.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gmsjzsuhb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gdipyzhye.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/grrjvwaey.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gmjrsomfz.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/guddjomwq.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gqptrdhjk.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gztcqgasi.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gwcweskhj.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/goagzjzws.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gpvqxixbv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gxphqplnp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/googkmhua.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gppjnklyu.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtqpudfgx.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gkrtpcznt.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gaffolxsl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gmpvvrrwc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gxxelwgxn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gyfkvsgdt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gqbnlskpz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gszgmxfhj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/ghtxefcql.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gfomxmayt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gotjqzbny.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gcqulgzeq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gxxbbplfj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gukolomkh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gtpdqbodk.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gaxcyrxkj.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/grtsowrzp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gpgudlbrx.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gmfcipsms.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gnfnbpxdq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gkvmqnhhw.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gsofiqnxg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gctwrlmxv.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/glkxnxghv.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gnhpkexhx.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gxoowebio.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gghdxdewl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gkmazigit.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/glmgbxbxj.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gnvswgexn.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/glrusvpyt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gelnhzksk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gwrrqczet.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gfmdugbfz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gzamlenhh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gdawbqnfs.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/ghpwvrqun.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gwsgqkczs.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gtxzdyscl.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gililewct.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gafznowyh.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gqcshpspr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gzojhmjhr.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gewhdzdme.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gkdkcpfts.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gyirbvyxh.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/glophbhsu.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/grvjbcyhg.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gbgrkgvit.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/grsklukjf.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gtgmtuhna.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gwkviyuim.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gxgthgxjh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gcuevbzxp.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gpxextgza.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gfrixlzhl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/guvbeqhdo.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gpnlsnrus.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gswzztnwp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gtuowqubd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gigkftwwy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gzghyyykz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gtjyvaidx.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gcylcqnqw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gwqdwxbyd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gbzaqqxlv.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gekeijiua.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/ggbmlkufi.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gsmqrqooe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/grmxtuoyw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/ggfstafly.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gvnuufmxl.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/geejvaxpz.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gxnfhqjxq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/gbgfligjw.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/gaprehnlm.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gwubnhsjh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gnizksxax.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gtlborbbl.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gdlyrqmxq.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gqafwjsjk.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gvsspjpde.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gsviihntj.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gskqiitwu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gralngpph.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gdyacdkzs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gsuvmhnhv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gxduadlzt.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gueuxwxwu.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gbnwhchdu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gockqkucm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gbqdsophq.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gzocjsyem.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gxodudawd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gkdyjfjmq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gtwqnfpua.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gzujrtwyg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gvdyittzu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gydeszstw.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gjpdhauwu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gyuqhmrfi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gtzgmaxeh.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gngnhrlmx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gvuhcqcad.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gjanlzfay.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gxlzgwjpm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gmkblbejw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gluxpvifx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gvbtraldi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/geysjbuge.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gnlxnwmru.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gorndbfae.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gbxuseciw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gmwxzrbcy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gtpglfbox.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gxfdygcub.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/grueihgdm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gdlypkbod.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gvdbzootm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/gjdhuufrb.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gslqprufv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/glmevghla.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gdrypzhpx.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gvychgqpu.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gtggwjowb.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gefwvpszj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gzzgomtkq.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/ghgryhtea.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gckvwkmhh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmfestaih.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gtzxbowdl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqrwbotcb.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/glymbhprl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gvbxfpqrk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gtkktbvyk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gbfoooyxa.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gnivdyrtc.sHtML


<!-- 参考信息 -->