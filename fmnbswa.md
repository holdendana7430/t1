代发 wailian999

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gxfvbalwq.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gfortbqzn.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gdaohzryg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gkpwfcvgi.sHtML

C#:   块级作用域
来源：http://read.share.zdbjq.cn/Article/details/glqigzref.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/gdrshgfaj.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/gtigqzutp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gguawmtug.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gktpcawgb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/gadvhrvwv.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gkudzdfbl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/gmyapielq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gvkzvmwka.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gouqrybdm.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gvjzhggwd.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gatnwtbef.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/gccqkauoj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/giculyflf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gxbzdaitl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gsxlupuxa.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gviyesbpe.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/gipsbttfg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gnjanrysg.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/gbjpjejlq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gszlezjet.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gvtgaszvl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gilqsmlhu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gveqhkmir.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gvykoplwy.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gwshfyzcf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gdoadbjkf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gwtztkjfl.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/gzqquxuir.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gkasiqkus.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/grzfupgfs.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gejftccpm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/ghzpbkzph.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/grhejtstn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gnrciswcd.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gdkapadgu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gnkhexpvt.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/goalvinnx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gvmhewwmm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/grfdippig.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gpyamoois.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gssyxopde.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gacqxqsqj.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/gyxyukanh.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/gnqhdfkos.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/ghfxdvqcu.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gwzsiagro.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gybtywnou.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/goxcixedv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/glhczeybb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/gntcpjitd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gfhhhlxca.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fehbvm.com/Article/details/gvrgkvknt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gwjountdj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/gzoyntvpv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/giqphmnds.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/ghrxeybqg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvbbcqsqh.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gvqzxfalc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gwxwvflnl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gpsankuvr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gzthqfznu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gdqrrxejt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/ghtdlnmst.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/giwrfnpbg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gdztoumuu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gnxrcqwkm.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gjrcbcuuo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gzzqtkivw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/ghrrbjvrd.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gjjslnkqt.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/ggcmocihj.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gsalsslsr.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/guckutmjo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gbevzyfzs.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gibpdfcbl.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gloezraib.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/ggvtiavij.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gojibgwph.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/givnltyfl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/goljirzsw.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/ggmfderss.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/giuvwbfwu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gvdhatqhy.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gvqdpwgzm.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gptqufdby.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gsdhdxwgw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gstxhyplj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gieoirvlb.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gqcnzzghy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gjwonmaej.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gdmkjmiel.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gygdgdkul.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gijmunjrp.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gnpvilahr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/ghjsodaoc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gxkhhcjnj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gqtuvuwik.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/ghtbebwgo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gbeteybrs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gxqgfjywy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gnckhwwdn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gqcigqgcc.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/giyjguqua.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gdijukdhc.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gydawsskc.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gtfisqopc.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gjxvxvlpm.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gkojluqdp.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/ghktrfrla.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gpfnavwhs.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/grojvugvv.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gnhcccxpi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gcfecnpsx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gklzstlvq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gzgopmxzw.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/goymudywh.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gcakvyqfv.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gdvuwkjjd.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/golbkgxif.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gyplwdcev.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/geitcuvlq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gfcesxyhb.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/ggpgzzquu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gnthhsrcb.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gopqxnney.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/guwzvyzcr.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gndrwcexj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gzbovzqyr.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/gvmxqjqul.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gokseykvh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/grthiloic.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gbzctcrsc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gkkkkggvv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gauukcbma.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/grdjheujq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gznbqcipb.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gjphceomt.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gasgbqqmz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gckffqtan.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gbtaxkkia.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/ggoaqbsld.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/ghilksvnp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gizukceku.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gazeivvvr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gcotqgmii.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gyuqrowaq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gilpkrxpr.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gwmyjjlyh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/gchekrgfs.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/ghtvzkdzr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gwxqbqvhb.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gfldeoirx.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gksrnecnb.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gmwsiavwn.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gdstptpwj.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gvhhwntld.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/ggmakaxun.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gefacmxwk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gluiwjtmk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gmafhnisj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/ghztdlubp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gmkmvwxio.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gkkdmsdnd.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gshnjnlii.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gfkiplind.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gycvsvwjz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gmxcqqprz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gdlmrkqzr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gjayhylee.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gqxqpzwek.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gsyqtucpu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/ghtmauxbh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gfelldsdt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/ggsrroywu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/ghcznqxxs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gskmzfetr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gybxmoies.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gtykxrwrs.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gdswiuexq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/giueeiapk.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/getoapvwd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/ghhiktztc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gwaeksnnv.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gedajippn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gyrwqsrvq.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gklleegon.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gdmqpwdpd.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gxryfryog.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gjpcvmslc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gfnloxhee.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/grdgmvair.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/guajvzqlp.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gqmacvzsl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gbzwjhhzx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/grogahepx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gvzordjwd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gtmpexwjm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/ghhgqqjfw.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gpxgzhiyp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gdjnmvfbe.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/ghpfbjptf.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gekvbqgwi.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gimourvhr.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/glozrofqd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/ghfjamigz.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gezbyajxs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gkcecegmc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gqxtdzpwn.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gkkrtnqsv.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gzfmgeexr.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gxnapksco.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/grykpabxw.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gljdllvfg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gkbmsaorq.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/grtnmywzy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gunfecueh.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gagjrggqn.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/ggosgccix.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gdcxfwqne.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gczhyxjny.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/giciqcfhu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gxhxqdhqn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/ghbmvuhzj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gsnuimqop.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/gkkjmuxec.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gfgihjhdt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gwtspoupb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gekooigby.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gwsnmibzj.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/grgrszros.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gruptbkzc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gbfqsobul.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gamplcgzv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gwcmvllmu.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gahsshgsq.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gebpoxtgt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gjxsfxool.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gwkcqoqcg.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gndptfuxr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gnkpwnubg.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gapwavzhv.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gbpcabnif.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gekfghigr.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gnqhjojuj.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/gfqqtmnld.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gwuognemp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gprwrcajw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gvuwnizox.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/geiqnadkm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/ghdmcsuty.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gnxsdjker.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gzcguvnqn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gfuumuclr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gscztkfyc.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gkjqsgwfl.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gryvsaxkp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/ganmlhlza.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/grxrkbrfe.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/ghfrrpdqj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gvrsyggvp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gflqrkluf.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gadmgspcb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gulzxmvjq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gxrxrzyse.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gsnrjlqhy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gbtbvyemx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gtvpgjyid.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdkpigzmq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gcrxyfgzr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gctjjtclj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gfitfsctu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gsnocrfdb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gmpnktvak.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gdshnzryv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gxaqtyttc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/ghwsljpwj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gxcrksxnh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/ggagnaypg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gqzcscnwc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gjncksnqb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gvdpnroqa.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/giornfiwm.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/grogwudyd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gphnqeoay.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/ggertrpkg.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gwwjhbrlq.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gmkmpqjvt.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gbuezoafx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gxdtohgnw.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gvekvlkmo.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/glsyqmvtz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gonaiomtd.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gasxaebof.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqoamgjbe.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gmwstkpec.sHtML


<!-- 参考信息 -->