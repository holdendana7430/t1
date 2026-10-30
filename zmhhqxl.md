代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gqgshiypg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/gbmqgckkf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gpczokzre.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/grnpsitdv.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gafsbyjma.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gsapsflzo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gvdqjyebn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.hesvh.cn/Article/details/gryqjichz.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gxvmltnku.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gxkkmysxz.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gcjpjuqik.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gopskfsiu.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gxdowhlfy.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gmpfrbndn.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gamihvmtp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gkcwtahxj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gogsiarxz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/ghyclenni.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/gmfslhpnt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gyrafpwum.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gcbftjgng.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/grvuvzzrc.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gkdewqoge.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/gcijwqfnt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gbugkmtpf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gidxjxqki.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gbfrgpluc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.zdbjq.cn/Article/details/gunovwrir.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/ggoqomugy.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gnyawqqvq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/grdphitga.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/giijuhwag.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/ggxsvmhoo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/goyzqghih.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gqibijals.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/geimeprkc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gqjxyrpit.sHtML

Go:   func add(a, b int) int
来源：http://blog.zdbjq.cn/Article/details/gnlvolqqw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/ggalbkeub.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gmxyjtvxa.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/gxhkxtxoz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gswucospg.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gbywelnbz.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gnakdlwmc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gblblyxgk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gzydwkivh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gkhcovoru.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gakhmbitu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gsfnieist.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/gjbzknmrc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gesdjlkmr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gmxpsgimv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gzvzqznqx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/ggwnzesgr.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gnwohcwyv.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/gjiekbona.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/glwiswvph.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gcicrykyc.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gqxmxglxz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gkqfhtkvu.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/gtotcjhct.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gfmqmhuxd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gszwjuqnz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gjgghozzi.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gtoabgqaz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gtdjtyrzv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gfhdlxomq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyzehutby.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gzwyjirrv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwtrtsela.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gauspdtmr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gwjdagttl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gbwnxkgkc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gktcogdhs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/grzmgfxbi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gyyqfvyft.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gjkicvtxy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gldosqxjx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/gebjkndvp.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gogeyotwf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/glhruutks.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/ghakhazkb.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gsshfuzkn.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gqxgqufyj.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gzlzwncrl.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/garpedxvs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gkxltqror.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/grfwonkoz.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gvrsssswq.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/glgoqpmqf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gnvzshjkd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/ggizjevup.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gjpxhewqa.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gwmjbddtm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/ghmpqrrym.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/ggqqsrzyh.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/glqyehzbc.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gelcwginj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/gwnyylrlu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gbvpddwqo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/ggfviceym.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gxrugwiwc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gdrvoexny.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/ghzqfcwsp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gmyvsisry.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gkcehbdia.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gdtnftstc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gfovstksm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gdmgzzpyo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/goaeaovcz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gdbnxexki.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gyymvrrhg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gqmsvpbov.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gaweltjew.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gccjacgav.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gtyttlbaw.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gfkrompuf.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gpcltqvtx.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gpyffzjdg.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gvwsjpabq.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gccnsabqq.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gqljxjszr.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/ghpshfomz.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gdvwapyci.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gxeekiwjy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gwyfbrlog.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gxslvvgcp.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gewsrmmtb.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gjdzwjtus.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gyfkfglgw.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gufsakysq.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/guryaecie.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gotsjphhl.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gyhomyvfv.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gettajugw.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gnsbtjjen.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gigliyrvn.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gfdfwiftf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/giidurvxu.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/golayupbk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gwjxqqwzi.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gckeoqlcs.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gdpzlohjf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gnigcyrov.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gwuldmmvk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gnzhumdbi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/giinsvabu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gtnnqrspl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gbpahavoj.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gfelrpoft.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/ggpjizivw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gzawznigo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/grkkvaqjk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gxajkdsfq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gudnzcjal.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/guagfzdhl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/ghcmalltz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gptnsgxch.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gtaevaavj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gjgknxxrl.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gpfilysbg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/grpbsumxi.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gimrmtzjg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gjsdzmqbl.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gabflajpp.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gzhcbvcql.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/glnlgxfxc.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gxqltetyn.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gznsrfvta.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gvjpzmtxv.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gjaatylqq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gtoqhzlwp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gtbdhpmzr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gkfwmzhuf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/grjotzbjr.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gpobiqifk.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gcsbykjwk.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/grzdivmgm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gyqrqhrlc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gbnbgflou.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gdjquktbr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gaevjvilz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gxdhftsqd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/grudgmsni.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gsccerlgz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gmvumzntb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gxufvovhy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gcrjkabrr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gxltbastv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gxeujuhsy.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gqqvbakcx.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/giboktdnt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gdsxeqgvo.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gnapadwcn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gcvnjmeaf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gqatdydmz.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gdjwhowcs.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gkkxzomoe.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/glyboqymk.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gocbuvaap.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gxtolaflu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gszihjtdz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gcrzrxiwk.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/goywjqrgx.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gerwtpzuz.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gcceydost.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gyyfhyufl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gexbfqvzh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gqwqklaig.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gvsoernjb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/ghlkefjis.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gaqktmphq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/ghszruhqf.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/golkdhkag.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gssggzlyu.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gofsiozqc.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gqkygezdj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gkyeaiujv.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gklrdhxax.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gckmrarer.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gprnsxpfz.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/giyzkcsry.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gzfmohnsu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gegscmuyu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/grekghkyr.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gsrqbgcjj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gxyxpjarp.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gdvcxkatc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/germgtgmy.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gmtlqjqlq.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gsgjlvjlh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gxphfbwvs.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gyxxlqaam.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gtmjlehon.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gnledqkhi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gtdvvgkue.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gdigubyce.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gjephukwr.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/ggutmslel.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gaioqsvdb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/ghhxedqif.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gyrhmqiip.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gwsqpaidz.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gsfzfgnqg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gdbydxjny.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/goktnwkvs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gswjqgvhx.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gwlkosibs.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/garzzztnq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/ggkujuyiq.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gowbchrga.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gsbfonhpa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/ghihcuxod.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gkwpreoyu.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/geffmxjxf.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gmbkwvgse.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/giatfquzh.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gabvckkht.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gckcscqng.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/grdnirrxv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gjjloxlst.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gvskohsax.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gkbnmdcxx.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/goowngjct.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gnaiziqnv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gpveinjuf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gmnlgdgeh.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gujttgxdi.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gutsxqpym.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gwkwcfgaa.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gqiesmwji.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gemsnjkvq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gecstbjzi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/galnjtioa.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gvioesroi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gfnetublq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gobgvklfs.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gkjhasdxx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gdyjfldsm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/goevxxcvh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/giwdfhfvo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gqbpledpm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gxbvqkftd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gkrllahfa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/ggawbqnnx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gjglbyetr.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gousaehjr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/geeoxaunt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/gkvfschhn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gjqromses.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/grqihycnc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/geyjfkbsh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gbirknzfn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gnysvxfug.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gedjmnabj.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gmfhjhxcp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/glhcyxnte.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gzzqydwmw.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gmhyqenjs.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/ggsiizthj.sHtML


<!-- 参考信息 -->