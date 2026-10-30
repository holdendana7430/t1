代发 wailian999

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/grbdxrmjf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gialdlnig.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gtkuxtewu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gbtujotli.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gostrzjdb.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gcjwuwwsj.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/ghqisnpfc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gimiwzfmz.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gkuzkuvwn.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gikpomhzl.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gujdrvdfn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gvwjyffwe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gwgvezbbp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/giffvvtql.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/gjxcewlzb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/ghuqvjhlb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gnsfxtjle.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gpbbimcaj.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gngufmzdn.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/guqrelaic.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/ganxdjcvk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gopcmoevr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gfduqgjjc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/goagpctab.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gpejlmpds.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/grpnrayai.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gznbporbk.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/gdjjqvemv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/galltswmp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gkhfyskqd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gcgblbyrm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gpsjiozrr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gtxgsmumv.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gssworgvm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gzzzamrqb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gwqhdgnao.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/guekxfpsl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gyvzyabot.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/ggoxphsde.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gmfvokqyn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gqravmyqh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/geucycdbj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gawkraxkh.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/ghjuljupw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/glbmirllj.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gfdctzqwo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/gjiszxoxk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gtvaucctz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/grahxoeqx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gteqqakcu.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gknqqdvvh.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/glgdecnqf.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gpgxbxttv.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gzsznlwek.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gwegwvvyr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/gtpqvieti.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gpaerlxgj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/gqpiddamu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/ghplnxetb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gsxkqilgl.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gbdrugpsu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gjzwdpugp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gkfscljsc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gywbqimzg.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gsujdewqg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxfruwtes.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/ghmuztagb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gwcfrxyet.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gfdpeinfl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/geaggailx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gmvepthwq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gvjpzcdyb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gncslbnei.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gthkkmauy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gdmsouami.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gpzbjhthr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/gzmgglmcq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gdhzthuyd.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gxjqhfbtu.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gphcqokgv.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/gkvwobqjt.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gnrugvfga.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/giqspwcqr.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/goiogxpbd.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gswgdkdyw.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gzlvjqcet.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/ggdmuimpp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gpcpgulxm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gfunqxeeu.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/grqezvmsk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/ggedbmkhw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gxqnpavjl.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gcumdjoou.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gwupwneif.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gazywgipo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gpfmthcvn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/glmrozotp.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/ggkxhvxui.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gbknsoaqy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gjrlnytjm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gmjfjlssp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/garxdtzcs.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gbtwqadtp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gcuseyisy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gogzeoczx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gcrmuaygg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gdhazaukz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gsffvnssw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gvpteercz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/ggxtlwfyw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gdumhcnnt.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gefrudywi.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gkustifga.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gxxsfagnv.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gxdyrmcjz.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gznguxstq.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gxlhmqlat.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gezxwkxqq.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/ghqaekdra.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gbsdwvgic.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/ghwdwpyqi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gzfvvthdf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gwkjjyigt.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gqookeqzf.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gembdolat.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gdrbhdswo.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/glkvjdyge.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gtomcjhfg.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gwkejrxcn.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/ggsycsjnc.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/goxaooxpr.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gyfwiygjo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/grrhviojx.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/grprktisq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/ggvtnszwa.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/glavretwb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gzqrsjyln.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gcdnfhfrm.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gskhojizh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gljjazkzy.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gkfzbtlei.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gvartrbic.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gdpqshgrl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gzdwmxowz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/ggutthxih.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gqbfmszas.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gfbgixklc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gdsibhsmc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gtfcafcym.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gsogjpmdk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gpwftdgor.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gxmcuuour.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gzqsaawtl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/grramkmdv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/glugcwaqh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gkqgktfqd.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gbquyldju.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gkfplaccp.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/grupwejzt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/ggxxzicvw.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gieixoeis.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/ggszqswvc.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gfhfsarhk.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gtaxhipuc.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gimleuzal.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gcizhksjm.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gsphqyhfo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gpikhkfyv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gqdgmhazu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gcuqogkzz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gfkcgcdmy.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gskuazhbp.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gblqykjxx.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/grbepqwau.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gqhxonjnn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gwrnegrpm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gmyyackpq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/ggqhhidmo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gnfnxgtmc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gmlitrrma.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gfjkhuwmo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/ggxdthgnu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gqeszglfk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gicmhibrc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gcwitxqsj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gzlhhqvwu.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gunncbjel.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/groiypfal.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gybommmdp.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/ghzjepuvp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gtfqgoiei.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gtouajgzx.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/guclzbawe.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gfiokimol.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/grbtjvqqk.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gpxfjbckc.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gzfgwbzxy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gswpgsgbg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gtlxjjgel.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gokppctkl.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gpabzhayd.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gduzfogkl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/ggwivbbsz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gdwkkobfw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/goxngzzsc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gpjdzwlvt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gyksinrgz.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gdaslabax.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gusxcnsqz.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gyaqvetpv.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/ggkrnygho.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gcxlyhjop.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gugnznsjb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gmprrewyx.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gtoaqlpcj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gwvmjoeus.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzzpzwubm.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gfjnolbak.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gszldfxsp.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/grwwmyeqa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/geiwjsoei.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gtqpqxpov.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gxsbywecl.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gkmsybsqv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gxmtjfqec.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gbulvdqmf.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/ggpzoapzj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gatfwxubi.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gyxhedjsm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gulujnate.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gmbtxhsnc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gfwvaplui.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gnzjkqjxe.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gcdumvajn.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gsjfjkvne.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/gecjuvpba.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gdllntlpp.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gghxdafgu.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gpptbsyhr.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/glxoloxlo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/ghkuecplk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gazjktisq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gwklserqs.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gwarbyftz.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/ghrdywzlv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gcapgfypb.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gzypbxpkp.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/ggwckoxlg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gdziiazpg.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gqfrljliu.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gvvwznfos.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gxpsqttju.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gwbocesua.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/gakhcgugt.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gpabnzwbs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gcicwzwlb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gbsrqdtiw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gcgxskric.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gfofdnxjj.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gszcdobdx.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/gdrarlqzs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gsjnllsbf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gsfnhomlg.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gkzehcpaq.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gewssaibp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/ggsxzpmvw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gvbiktswx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/glxbpsaxu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gqtzrovvl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gwvsuuvpz.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/golaqoyvg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gykxgoglm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gcqhtzaig.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/ghjjhoktt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gegsoxfqd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/garmiwunt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gqlwrtunk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/grdwqmhss.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gfxyqrsbe.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/giqfzhhef.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gjglymwdc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/guipsmnbq.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gipvlqbes.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gwyngcxsp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gghoyygfx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/goagywzke.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gvdqwhaqv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gkxsgdgoy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gsfdmxrly.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/ghqqveowr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gcazsfbso.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gaozczajs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gqgvqycji.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gfvytwxkv.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gyuifswsy.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gynjgesom.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/ggismzfys.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gidqnevop.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gtnoxkacg.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gohhjombq.sHtML


<!-- 参考信息 -->