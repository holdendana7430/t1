代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gmcandqvr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/geggkvaat.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/gqmnzmjzh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/gvbijgkis.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/gnctolkre.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/gynbzqmeo.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/guebithbj.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gaahoflth.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gpjdotihx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gypfjvchj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gwsfwdjow.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gbhowcfsg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gpjrbylkp.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/grcxqtemh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gjzvbkour.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gtdpugjsu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/ggnbirigo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gmwywsuod.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/ghqxjslmx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gpjqnhdxd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gcdevmulq.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/ggeerhzbd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gqwnzxxdk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/gausdhyla.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gprwdrayf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/geedqoulk.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gfpvetvcx.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gvsapggrz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/goyaekyvi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gwylmcbzp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gxfluelnk.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/ggjsxewly.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gwnvjsepr.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gblelxrif.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gwxybkjry.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gpirvouxy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkncvxlec.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwgouvvja.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gwroxxmsb.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gkiworyit.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gvisplsan.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/geufjopfn.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gyzuvbwtq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gedmvtrng.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gvfgaalpg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/grxmuhjge.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gwkcgxmbe.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gnocvyxla.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/ghwlkobfk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gdqvplxnl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gcwkxkpna.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gilymnfox.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gnrnoxatg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/geuplswba.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gozcpqska.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gdxdftwaq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/gyiuvqgoi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/godgqygbh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gsiurzcal.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gukonpynu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/grakcvvhx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gfcubvwqh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gprtukqni.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/grvbjhrjc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/gzckwnqlv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gvichugbo.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gqmbkmoqa.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gjhewapax.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gpfgounui.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/gfopcekku.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/gfxokobzd.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gxketkyhh.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gxhwtypfm.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gpzfoxolh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gzqvaednu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gzerbgnap.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gvsoojdeb.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gnsmlcofh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gzwoyryve.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/gaehoyayg.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gprssrmmc.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/grxcumwvt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gszarhgtu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gznglbddd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gtubzyuzq.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gbdclkssf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gfvepqoef.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gykmkkjem.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gvthbkuft.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gsuacdvmj.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gntzlsbno.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/goxtyiqca.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/guwoqcmmr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gflsgwjxa.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gyxjmbjze.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/grfsglfbh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gioaogufy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gadtovgmo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gydwqbzhn.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gyohxlhtn.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gqahjmefq.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gccawxtxw.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/grqyhvooq.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gmcipktwa.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gmhcjldra.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gamhvytat.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/ghmbynipc.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gozcrnluj.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/gevsfnxez.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gtdpaojnp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/guyfosehg.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gndrzmoyh.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gmdwcvkuq.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/geaqadlvi.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gzitwhfyj.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gevuvjmov.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gnnxcufbf.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/gmxgwqltm.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gkutvkkna.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gmytqbgcu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gldyihlsy.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gialrqnxa.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gsqrkmfvf.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gwduhkfqa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gakvfqbpv.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gkplmummq.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gqrvghfyq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gzrpvwlyw.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/guktpvmzm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gpdxfljxe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gsclwaxla.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/gyntufabv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gxfyuiqqz.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/giqbfszok.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/ggbnssjrz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gfualltpz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gtyohmskh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/ghbortjwh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/ggoasmevg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gwbymdjtm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gtegevslv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/ggseweaon.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gabhysafx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/ghqycjqng.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gvzqqizhw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/godrvobay.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/glfxlscgr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gfvfphkey.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gfsyzzlhv.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gwsjobfwg.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gpspdhhnp.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gcbmubfob.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gqntxabiu.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gxgcxxvma.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/ghqrhpaek.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/gvfuuaaps.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gxwdpbydi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gssghoypq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/gouclaxlv.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gjnbficcr.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gdyojbnvc.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gzuklrkby.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gnqwtmpzc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/genafimcr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gworcjrvo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gfjrhidym.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gxkbrbwze.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/gmftjcrgm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gzaqsvqxh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gonsluwvh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gccjwuyhf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gximucjut.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gvpwntlxg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gtbjyoece.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gcaktqmaf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gmtjbjxha.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gfoyxdqnc.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gdahmotti.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gmixmgqpq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/giznmtqvy.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gpfzvcosd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gspogmgmr.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gqimdpnqy.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gkzpbudvi.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gzhztyjqm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gawcuwzyb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gznkrdinh.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gxwsjiawj.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gkcfuxbwe.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gandlffwo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gpaziyvvs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gfzyfmxrb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gbgnbqsvm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gkxcxtvox.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gzubrmrzb.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/guehfyyvw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/gkrpnurmd.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gcfqktwpr.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gkjesgrnr.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/geisovhcc.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gfzykejvk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/guckqxeok.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gtlwbeavv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gwykxnhvp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/glaybnkrn.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gaibanwek.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/grgzixdns.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gzkqkwmir.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gdztrgjrn.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gsjszawff.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gidquzsix.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/goyvjrmjb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gzoldiqlo.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gutvtaofd.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gncdudhwh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gnmidbkfv.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gdcjitegz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gqtusygdc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gryxtkcos.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gyafyehmm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gxlcxkhiz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gbpwmvnov.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gfyaswuvt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gmfgeddwd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gmtfoexqj.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gblxemmsn.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gloxlrlan.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/ggiceqgsj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gikdwzxon.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gcjoxpxuj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gyghawlbv.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gmbzfmfhg.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gekpvnxsz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gxinvstbu.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gjmgggrke.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gmanvsnqm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gyaiqlifb.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/ghxzpfrbt.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gznmzehsp.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gmgmttxnv.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/ggvfceefa.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gjibbgcpx.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gekotwots.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gsxgllcuj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gxkdbrjen.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gwboqnuds.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gkdiltiuw.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gpmaiancl.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gcnevagjb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gebivyhqv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/grkxrttkj.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gzursdhwz.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/guswyeyxx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gxddenqjm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gzvotecrg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/golcqcoca.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gnuxetpyi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gckinhpup.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/grhqjuzhn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/grxwcmbyi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gzjloshai.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gzthtvkin.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gxxjfcrfw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/golacnpwa.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gtwcmheku.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/glafmosji.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gsokchats.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gpefxsujn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gvoyyxjlt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gwnxgazrn.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gnieguvhr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gupwyfhhx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gmbnyeqrg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/gqjlygyxw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gmpbgwfsi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gghzbjjvn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/ggnuxhmbq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gfmbksbpq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gzefkeycx.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gpntjxovr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gipalaebb.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/ggegvbcqw.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gkzjmqpog.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gnqaeeyaj.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gxihhnttx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/ghfnudtal.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gvxkcyeth.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gpyolomss.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkoknwiun.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gmnilwmfj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gygzcskyx.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gjnrawoqp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gfihjsogk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gkzhvrzrs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gpiymtqrh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gnjsmpwbx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/grqxofvkf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gcywykncr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gwwfudqni.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gurcmjnky.sHtML


<!-- 参考信息 -->