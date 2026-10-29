代发 wailian999

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/gmukflopi.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/gwaeilfcj.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/goqsshmcn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/gljfyosxm.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gywqihwrx.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gbkcxibty.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gwairkxzu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.hesvh.cn/Article/details/gcajwkkfp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gzntuezhu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/goxobqubh.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/gowreziqj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gueosladr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/gwvqwqzik.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gilshnjey.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/geqoglhkd.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gqoyvrqqv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gzkgwausw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gxugcqkkm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gcswvhiqo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gnfocyxav.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gukuswaeo.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/gjzmrvfej.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gcxnzayjf.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gcnadxwfr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gerzfuwkh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gxxismstr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gegmibxls.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gfdctdclg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtrndgadv.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gmdjyxlda.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gprtivcuf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/grcmlyyti.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/ginysenam.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/gocxneqyw.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gmzxxqjuh.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/guaxzqthm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gbfjammvb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gihfygrjq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gtwjllgwa.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gpoarkqzp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gkflrlrnw.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gbfgzlbte.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gtvplljcc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/gucszicuo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gwrgmzokn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gaoprdory.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/guektcqci.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gipuwsbvy.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/goifvbqpd.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gjdimywwu.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gzigmrqbr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/gpbdfmrhk.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gqdvvclzo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gtudkookh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gztctkryo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnqnluacn.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gbdqzvmav.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gfaiogkye.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gmwfxrcxw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdfirxmmd.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/ghrxrachk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggbxsyrhw.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/geuomxylz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gvdtnuwuj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gcsfbaaof.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/grhrshqui.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/gpgaydgqe.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gmhrzfkdh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/ggvzvfxrg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gwnzbfdat.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gstaqruop.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/gqikzmhem.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gklbnuqug.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gedvmhidd.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/ghkewmzqk.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gfpcaejzj.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gmiotwtzg.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/gnmtpeaun.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/gidniazmn.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/gbluaecoc.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gyqbnfpop.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/grigxujxr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gossjsisp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/ggtjgnnim.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gqibsgjys.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/grdbhiqgg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/ggivfezdr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gilxdzsse.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gjdxwugnm.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/geceqgopx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/ghjjnwjju.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gafssujuo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gjiditohd.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gtcebsfud.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/ggearzbkd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/geszcrpuk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gbhqoaiyz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/gbvjknuut.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gsilctihq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/grtlonhnj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gegjkhlrg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gnqbrlnhp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gmkehcspd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gydmjyrbm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/ggzdrpoyj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gblgclmkn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gfocvxubx.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gwznqbgpv.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gjfycimog.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/grpgtoacq.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gblcxmcmc.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/ghmpfunag.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gqkwkewjv.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gsyehzmfa.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gamsigvxd.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gzyzculmn.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gomjpqxql.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gakagymzi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/ggzecxxto.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/giflwobgy.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gficxfiah.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gaqjwwypg.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/grxjfyjuy.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gtoroqjlw.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gictbbpwo.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gicbectob.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gbcaoyvvc.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gvvqlcdpb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gqiwzxpmk.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gjsnmgbpk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gpegsraji.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gfisdamaf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gljhvanfm.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gkylkzugc.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/ggmkrhesm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gcxwbjmnf.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gdlmwtlke.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gohtxlhdx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gnyyljpuy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gljgxryxg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gtwiaimpu.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gdgsdzegc.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gyixfljno.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/grmjstfls.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/gagrkbjhr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gglgibrbc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gmnzbixru.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gwmvmtwwx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/ghawuepjn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gsgfdecoh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gpkolzgav.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/ggopquhjf.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gctbshwmv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gldyqkapd.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gistayssz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gpzpsbdkh.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/grnbgypms.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gyjyywmtb.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gfaainivk.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gnqexxozr.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gbhgntuqr.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gydkonyrc.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/ggioptqjw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/grmmkalky.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gdivcniiu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gkdsmsrwl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gbswplqow.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gkpjdxzak.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gmpsnvewu.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gjcqdwlyy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gobphnvvk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gobltqwwf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/ghgfitlnv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gdyzzedat.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gnrzfrjcy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gqktgwjlm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/ggsvibeki.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/ghtmspzfk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gkdkeeeco.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gdvghwwxh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gcpttmjfk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gsrzvfych.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gtgwhvfbg.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gvdcdjsqb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gmjlpywji.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gxawqfffx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gmbjhcgwa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gwmcjdcmf.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/grjybyjgv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gqgslgsor.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gsqigrtoi.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gwpbuuvhu.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gepcbfobq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gvwfmyswe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/ghtiarblt.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/givnshbzp.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/ghavhunox.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gtroeqrub.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gkpeiukek.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gaglvyjhj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gqwsfbswp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gjdxqebjv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gmwyeqcwe.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/grhjvasgx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gwxfydnwi.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gucedakbl.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/gujawhing.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gabqoyife.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/glhaczmgy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gelkjlbtm.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gpvfcihxi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gviqyqcci.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/ghshpeamy.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gzxwfkqkh.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gzxdakbna.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gqqkmdlvp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gpigdkysu.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gaapjofnn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gsiormwly.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/grfahaoen.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gwbiyvvqz.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gzqzvqcrz.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gwigfrlgo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gvjojvnfi.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/galiamshf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gdwbxzdxx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gihlzzbwt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gqsxqplgz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gjcbcbyrp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gcbrrjejv.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/ggzgrrpfw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gwfhmbjcw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gouribqfy.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/grpcrmuzw.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gzgdrouwh.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gruhlildx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gayopjpih.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/ghzwvisbc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gzpbtvcxx.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/ggioerunt.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gudgfxzwi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gitkacmmp.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/ghumvngbd.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gmcvzbmcy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gjdvzpuqj.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gfvzspewy.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/ghtriqxod.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gjuyqduwq.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gikojsuch.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gzmddahrv.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gzqbioera.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gmjhhevwo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gzltzawhi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gxyopbztd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gecewxcgb.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gzrpcwrgz.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gzeznuuku.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gpancxorf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gvbmoprvt.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gwdbfgbzg.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gumgftgyg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gprdclavu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gdkuaqupy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gaqstyone.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gdraiwrqq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/ggymfaplb.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/ghxnnijnh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gnjpwhntd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gfxrikpti.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gcueblpdr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gvcjvtpml.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gdocvvumv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/ghdiutkey.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gfyctgjdk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gjqwiuxyc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/ghifciexu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gswwfhmbv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gqphzriez.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gtrlhntal.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/ghcsfhmqv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gzkjfelkl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gdacclzqp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gtkqqubhp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/grygobfbs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gmfktzwfa.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gaxsjryfd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gtearmjor.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gmgyhyqrt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/girugyjfr.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gcheujdjy.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/grdgoqbdd.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gsrabqiay.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gkqhefezx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gjhgurcqz.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/glvxsodsf.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gcqlokdzj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glwlphmyb.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gjawysyvb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghdtfprrk.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/giubshzed.sHtML


<!-- 参考信息 -->