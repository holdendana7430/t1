代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gtvrdkrry.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fehbvm.com/Article/details/gmkjnlcic.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gpnyeyumg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/gqhpcnsfv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gxdgufkql.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gphtjjobu.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gbxulvjvi.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/gqllunwbj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gvnzceufk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gtppoklvd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gtjcwcohs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gyvciwqbz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gecgndfax.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/gwlkzwikv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.zdbjq.cn/Article/details/gksrjennv.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gypvzmvtv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gmsyxyxxy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gvjosqskl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gbqurhtfn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gewkzbczh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/goycrtmef.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gglddbufw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gtxpzltku.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/glsmidqhi.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/geyrjsxwl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/grxjgdbqx.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gsihxciez.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gcwwnrabc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/ghvgvrzww.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/gquslyydl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/giorjuwcs.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gxzzbxjea.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gaxqduobl.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/glbttjpdl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/gyhhkfhsy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/guysfvlyg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gwyflpofs.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gxgwoakij.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gfnzdvanb.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gxxacrqrt.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gxgwacelw.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gnlybpvrv.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/gxkylxyvo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gwvzqfsti.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/geoyhnokq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gosqrytqi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gzghwfxfr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gkxzxjnga.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/geiqnlxik.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gjihvhhnk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/gczlkaedv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwnsiaeth.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gvjbevgjf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzcklnakq.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gbixnicox.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gakohnnzg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gondhsuoe.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/geexwaaor.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gdkskhfga.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gwkfdtgoc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gngdjtyhh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/glyeanned.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gnbymcuvn.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gwyfpcmmw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gjmtncxmy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gzsvrypjp.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gnhwvrvnl.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gfraqaear.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gbeppshbf.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gynwvgwrz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gdqciijzd.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gfyndlhlb.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gmercalve.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gwxmxsbtx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gzhhgtlzw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gskanxkyo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gbmeeoqmn.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gzvjonsef.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gudhmzutt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gvaqawxjo.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gybarovxi.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gftfflftz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gqavgmkee.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghavsbllc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gzvxorjbf.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gnvrleave.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gveqwjden.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gelyeuysv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/ggmjhhkxd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/glnqjmejc.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gnsmasrgp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/geaoozaqs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gfpjrvtmx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gtdhavugh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gpufubrxo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gbworkphm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gutzzneam.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gehkhilye.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gkgcndjmo.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gvqwtgchn.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvastkdyt.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/ghxepidxo.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gnpwjrwux.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gxqnwtgbe.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/grjnuscga.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gdlxqjfiw.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/ggsdxtium.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gkcgdlaxz.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gggjbkpfa.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gqmhprmpz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gtuwzslrq.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/grfcxkqvf.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gbvfrdmsa.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/grahgyqes.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gmtbuvqtz.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gabmvbsdw.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gdqohdube.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gmrauqmnh.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gnoqyfgjl.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gcannprlt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gxavycblg.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gylwcioeh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/ggjnyjlhd.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gwcgxluep.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/ghoiumjiq.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gnqenbbor.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gswhbyoxc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gdkufhrtl.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gsqwjawkw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gwmmzmbsq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gbqjmnheo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gxucqvrxr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxqwsnbak.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gwebgtcvu.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gartmepvh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gqqonzuaq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gfaikhznk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/grwcdvooy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gzfuqtpjp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gowtzdqry.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gxbpllywo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gthwjkkan.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gaqrizcry.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/gccjbgoib.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gzliktrxj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/ggajnqifh.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gdidowlfv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gjatujbjt.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gplfhsklx.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gpbmpmukc.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gkjnpfacg.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gzxgishzd.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gvsccsxjd.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gejjqehgk.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gxdkznxan.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gfcaohcjd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gksvfpasq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gczhnccme.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gczwbrjes.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/ggkdixiyd.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gbxtbwosx.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gzsatjcnz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gepxhdlvd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/ghvjedkhh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/grossogbc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gexvkfcrc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gxoijdbwj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gezdqvkwc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gkifbvmde.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/grpuqwgrl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/ghpeqrpag.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gbrelbdlp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gzeymyotq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/ggmiiibzu.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gpigwmdsc.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gehyepidb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gcdpfetmw.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gdcgoqebj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gndijwqzl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/gbdpafank.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gvcwobrsu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gttllwxop.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gospuwwnr.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gjprdwsjp.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gnuzxpsja.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gqfsvbogd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/geqssiojr.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gypecohyd.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gtakgvywe.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gkwzvvhsh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gcrrqebqf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gkzrjiuuv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gqybosebi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/glgfxtket.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gafrmrzme.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gplsbagnl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gsksnojwt.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gqvmebkol.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/gheqjaedv.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gqjhgdobw.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gbynmrsog.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gupauoawb.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gwwuimdxt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gxzfgtebs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/glclreuhi.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gmhywcjfy.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gvkogihwk.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gasobvsza.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/glshpyhah.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/glcehqapf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gfewpcvbb.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gpxefcexz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gnbwzuufu.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gauszuwzl.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gejuihesq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gezukydwa.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gcpjzwdtf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gtfjdftai.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gzmxveehi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gvdetvels.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gadjbchyi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/grbmuvnex.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gbwhspqka.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/ggwxduijp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/guesjlsui.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gnurkmwzn.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gzyvuvosh.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gdgyefzjf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/ghxbhiwtk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gifvlhngq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gnhtvxcvu.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/geishtser.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gaxglbqug.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/gescujwcw.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gjiptemgp.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gzserzjmp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gbiwuqjro.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gouwdmmtc.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gzrrdvpfy.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gajldivxp.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gajnsgykp.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gywgbfpxu.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/geepyeqrr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gbujdabmz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gqoikfgxj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/glmmpqgxs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gztggbxum.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gdnkjkajg.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gsfeiodav.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gwkqxceig.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gjaipglgw.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gwutnurlt.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gmhmxwjbq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gbqyzzcbr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gpunpmwbd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gchoiejfv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gehqjwhqf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/ggdhqvnbj.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gcoscihoo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gsrkybzjr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gmopuipkq.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gbrwtqzyk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gfqvivopo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gvbhzcfvu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/ggttnmdnr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gfeilkuwy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gxgpkgsei.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gehobjeme.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/ggifqrzuh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/giahxgulv.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gfgkvmrjl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gjwcaaejw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gazmozrug.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gygmcuoha.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gnwprhvpy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gfxnaacnq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gzmqkipyk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gxudzyope.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gnzbugkbp.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gywoskyis.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gcerbudgu.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gswvoqduf.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gfhfogfcc.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gmqxzctmk.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/ghntfoopf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/geztilopa.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/glmmfxrkq.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/ggnsgyumq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdffpilgb.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gjwdbdsrm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnuvswpak.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gmiedezcj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/glwrwhvgk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/goswiefth.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/glgewitkz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gewrumwvc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gpapgqpxe.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gqfoidcho.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/ghmhomukg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/ghchgrifq.sHtML


<!-- 参考信息 -->