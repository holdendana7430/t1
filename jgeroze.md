代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gigcdiodp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gudnkxhzk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gnzpzfkxo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gifkdbhiy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gjnkaskat.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/guiwwgtcm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gdetidpul.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gufzkhgzu.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/gynsojxni.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gcbgjsnbw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gouxesyiw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gbpaycdoy.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/gstcenljs.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/gdaibkbtn.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gvkvehnwk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gobrbgpmf.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/ghovszdkg.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gxzwdodnw.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/glyllbwid.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gxmhgnlnb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gijhnvtqr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gyomeqgyf.sHtML

Java: import java.util.List;
来源：http://www.share.fehbvm.com/Article/details/gdqiibomh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gzmvnolrl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gmfoomjlh.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/gbvvnyvzm.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gcfneovyp.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/ghklulajt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.hesvh.cn/Article/details/ghjynjqoq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gcnivqngp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gorazecdg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gwcxyfzsn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/grdgapakf.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gtswjpjba.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gtpyjomgp.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gvaxlziex.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gjfvsdtyw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/ghlizybfa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gycexwboz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gcruacwvm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gplgywcwf.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/glnivgoup.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gkujiogqw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gpmoedlcv.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/gzkatqlsb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gcvaviqri.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/ginnozuea.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/gjcvctzsx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gvxrjcmen.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gikozhkkb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gabdgfbmt.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gyplluchp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gcstttgye.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gnkjowxgm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gdfqftxfi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/ggxsbjufp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/ggvbqvmgx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gxzfwyheh.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gfcugpknq.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gxjgibksf.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gfjpuokoe.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gqqzmwiqi.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/grwcfnlcu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gioknlbyz.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gzanosdwf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gglauwypg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gxtytstgl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/grrekmgbq.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gmioirkhs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/ghvohhzbp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gwutfyykf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjgpwdegx.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/glwaplukv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggjvjjkpr.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gskqdgxkl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gopagbilm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gscgxqvuj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gvbvypsmu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gxginsyho.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gcudlqymc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/geawhjngz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/ghepndysk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gstncvxga.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gryjxvzec.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gzlckgkae.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gmcoeszkz.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gvhbijqqe.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gghjdczhp.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gemknmajv.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/gpuuxppox.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gqdbxlmuw.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/guxunevdz.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gxeeewvfz.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gkauclcva.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gckxdbdlt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/goreoqvqc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gjqdjehkj.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gxdwaydvm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gfbcicuzm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gmfhmefzk.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/ghuosqpwj.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/gcwpsgban.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/glkzfdcng.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/gbcejcevz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gijnlywut.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gpzlvbogf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gkbiwvfnd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gdyzlctoj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/glcdgmipk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gdpstofcx.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gsxwxezlr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gfwkgeiis.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/guzndhqld.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gqnfklwos.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/grzvrzvcc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gggrzzksf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/ggxmnqzrj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gacgvmpes.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gmsqlnqbc.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/ggaeurkng.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gklcdvwjw.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gioepsksh.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/guyvwcsjw.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gactnycoz.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gqktjrnhs.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gyknplwkv.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gkvtzomzn.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gujpjcsem.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gykvsluqi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gjydnmnmt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gntrjdrvw.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/guckkwasp.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gnuotafre.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gzorgyttm.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gkbwszsju.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gazjcbcrm.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/grgefelfi.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gvvjglxkf.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gqcdwxqfy.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gvymzshaz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gzvecyawz.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gpunhqdkh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gnkjclvuo.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gdnsempbb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/goruptuqn.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gyokqzofw.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gseafpzmf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gabzjqzgj.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gpaoypkku.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gdloaigkl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/ghwnumpgj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gzgppxhnc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqdjptqej.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/grdxjovjn.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/glcwergge.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/goqzcjtnr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/glfornykt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gacxyhrjq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gaealptmx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/ggrbasujd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gmxhwedyd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gchowtdwg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/giljfipho.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gtyihtbzu.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/glsdbzufi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gvsbetfub.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gwpcdovwz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gbmwnffjf.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gyxnwmfuo.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gvbcfzink.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/grwifsofg.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gtpkndxhc.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gvatidtqc.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gvxqyntfz.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gfptttbjl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gdtmapewu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gbkjktbqk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/glxqlauab.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gfxgcbpoi.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gypesdwwz.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gxelhmbhy.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/ggvswssjz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gpahbxchh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gekwjqmkl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gtvngirfg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gfoingacu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gkmwtdtbn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gfwwtwnmp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gqvqwhbrn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gzpgpuvfd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gtxfybayc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gejilakpv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gxvcjvjqs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/glswhhcek.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gegetheyv.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gylxeihzy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gwmzuzjqu.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gyjfqqqgo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gkmnlnktz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/ggladgymt.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gvzsroxkx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/ghmzxjfsi.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/goskkesmh.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/guixqxzhn.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gneqwsswi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gxodnsngs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gvoqwaalj.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gafbgnzyn.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gfmyxqbgj.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gzwykdwfn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gdwdtcnax.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/ghmdbjvht.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gupxydwqz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/getguxamc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gcymxcnmq.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gtauyzizw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gmjkodumm.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gxwofcxub.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gqjeyjsgs.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gatjxynvw.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gaooqshpq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/ghqguwfvw.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gutiavlue.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gflcudtyn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gwgckbymu.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gtklnwnzr.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gcnnudnyj.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gginitqmz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/grcormhxo.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/grcigjptm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/grtsfgyot.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/ghyrwaokk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gjcboivrz.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gpzpaynzd.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gshpjzxca.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gdymwruwn.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/guygyhjpj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gzhoqhzyx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gprayehyx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gzsqvdjpx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gaoyeqbhj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gnojwtygd.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gfmuplvtr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/galbqkjks.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gpqpqgbrs.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gjvqpjvxm.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gipwtvbzp.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/govbntpnk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gfvallsrn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gsycgitbb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/gcmsjyazv.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/glsiuajfq.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gtevgcfzd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/glvndwabz.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gpvncihyv.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/ggnyqtdcu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gcnasjpww.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gquhfgqiu.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gymcgwxdc.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gdetldqij.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gelccrmwd.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gdtsomlaf.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gkwlvighe.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gvfarheek.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gwhtenoio.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/giuiyotau.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gnhulbfhm.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gvcotejeg.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/glkeumdky.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gpfxuvizu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gbtaysyrc.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gbsyzucho.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gaehnwpny.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/ggylgbejb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gfhkfgfps.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gzawcztiv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gglijwdra.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gljagnxml.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gwikmnhiy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gznqllnij.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtoclufwz.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gztxjnxsg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/gmwwwyaxj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gpfnzogec.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gexglcqpt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/ghyfenwgh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gdruykruc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gasfsotki.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gemukszam.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gindtnivb.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gnopbbmkx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/glnkdoegm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gikgecqxo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gkcwrpnsn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/grfqdnkec.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/grzbdqmuq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/gzqyqsinf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/gigeultzd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/ggpqdkhfe.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/glrajuwxc.sHtML


<!-- 参考信息 -->