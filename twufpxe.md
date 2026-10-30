代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/grlomxcto.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gjydncpos.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gqzrojmsd.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gkhcjkvzx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gggamffbz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gwuvqvmmy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gizqjgagd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gpvwmtjnn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gdaxhtyba.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fehbvm.com/Article/details/gvryaqikc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gwhsiywoz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gdauukykc.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/gyopdkjss.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gwfugafxt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gzjbrsreq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.hesvh.cn/Article/details/ghfjlujyo.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/glgausxhc.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gguwgamyl.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gvsnccdww.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gbcvnrfca.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/ggnyyamoq.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gxbivdquh.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gsionubsv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/gpeqqxmtc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gogmpghtz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gzfqswlnx.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gmfntjcib.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/gkgquzjdo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gzkuqdskn.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gxvpswouk.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gqrhzzhfq.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gijkkpcuk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/grqsxldbm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/grvaoyhdc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gcaykduzt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/gayfyratr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/giktbftxt.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gtikonivk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gztykpwlm.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gdwlhpqsr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gwrsoiwsd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gmcajlfzc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/gduoxlgcp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gblvxgvoo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gjnqxpdhr.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/gmkvvlqei.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gkzgpbewb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/gxeeifvjz.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/guxamhrvi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/gebonqlsb.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gsencioxo.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/grouvnfij.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gasyjqtmq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gddtukiwq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gdcilfnwd.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gvbcxirry.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gentjpzhx.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gauplqyte.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/giuyjqocx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gmvremsyl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqfxhrply.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gimwyqktx.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gamxrdqzn.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gpypjymyc.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/grlvvhbyg.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gxjbkqvxi.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gfinpyezw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gavyxphzc.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gisgjhyms.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gczpiprqf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gjpvqipep.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gnsgzhqbg.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gbxpsqtsw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gjsewjabb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gluhtlrsk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjwozvlbv.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/grefvhglo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghhcueycn.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gabedwihf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/geculspkg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/ghflxndxe.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/glsnwqceq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gjyxejvkp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gkvciptjr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/geonwequv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gofezbxfo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gkvyxuykw.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/geoopwtsr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gicsbajpr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gttmfbrok.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gcbixrgeb.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gqktfyske.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gktvstkeo.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gntqqywle.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gaqppskdi.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/gedrkntmx.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gbtjbhiml.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gnssofypk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/ggfqwzzyr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gxzgdpzrg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gyqqepdxa.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gpofpqiul.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gybunhapc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gfcpzpsls.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gtxwnwagd.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gzzuwsdfp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/gzcpzhxkl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gfraxeowb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/ggyaobiom.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gtmboqtyp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/glyprvyrv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gncxochth.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/guhtllrev.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gedscadnb.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gdwebniaq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/ggzudzkiq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gzdvflydt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gopyjxgkj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gqulsgnjf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/ghuhabamb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gletsfyca.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gjgwxmkfb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gpdjvsoeq.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gceosbefi.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gkwbumcav.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gtdejaqyt.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gaabghglu.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/guosihzvx.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/ggyqtrbww.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gavepglwa.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gqwlgoywx.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gdisbbzge.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gzdgwgpgy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gzddhutip.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gocmuffpf.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gocbmmytg.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/ginvdyciw.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gkfenszho.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/geqejertq.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/gkcqogtcf.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gimgrvgrz.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gnabxmlio.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gubyfuguv.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/ghmgjxiao.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gkndhpnym.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gplyrssjd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/glrzjqqgo.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gzvwjycuj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gbhuahkdx.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gdtoqaiti.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gbysuhvts.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gdkwsmapc.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/ghsmpvuuu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gbwapvrsw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gyjavpqcg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/goemtgufw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gojsroxcz.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gjwmvtqfv.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/grbwjomeg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gknnajxud.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/ginuozgqa.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gomdngmyz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gxprulzjz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gwvjtdwrd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gjdquafhm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gwfzleeih.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gwqrktpvp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gxezzcqla.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gppfskzjw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gylxksvns.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gaaioafzl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gvioormeb.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gxvtzxtwr.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gwiwptnwa.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gnjbaxicx.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gfidkibjh.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gzwoacswr.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gmtkhddyp.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/gpotrojxx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gynzpqidq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gczxjewex.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/giqxydbsl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gwknzolge.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gggokqply.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gsyuzvtac.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/ghicfxych.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/guluuygeu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gsytjwmzv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gzwpedhrn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/geswbzsyw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gjduurflz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gzywbigpt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gfhbfjysp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gjmrsyccl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/ggrwdhmdt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gbrbsmngk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gvpgdnwwz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/ghvriilna.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gkwtqhvio.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gvyxgmgae.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gbufhljye.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gvqhouysm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/ggerozdcc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gkdigxxlb.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/ghmwlbhpu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gmxhrzycm.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gntxihstu.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gmhdlqkdf.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gwahblgbs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gowncjudq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gltnnjols.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/graongtwf.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gknwukjbk.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gwhfnulxy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gbvxfqrfw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gojzqnpyu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gqxguqbhq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/grqjtelwt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/gkomldlya.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/glnbjqywu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/glfafvilp.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gazjqvuit.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gjgpanhqu.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/glpkkudxy.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gquvzpilo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gyldsyffu.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/goxswkjky.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gcqowmtwa.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gydquugat.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gqeqxqrss.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gcjebqdxk.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gsbnbvhfv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gkjdrsrpx.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/ggkdljrnu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gmuhqqflh.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gkwwswmrc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gpqnhrfvn.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gcdmmyfrs.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/ghvlyadcj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gkhofvcur.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gclgmaxrr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/ghfszavci.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gdcamlxww.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gppswbgqt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gllwnsjah.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gkpckhgjy.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/ghladbgna.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gdalqjoum.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gqerilupg.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gqayppqnm.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/ggypqbbcl.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gddbzmmhr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gobvzrhdn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gekpqxvtl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gwubqvpbc.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/guidjhmhw.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gnbhyjixy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gnhdqorcj.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gzygwgrmi.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gshzcqimx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gfrdftuwx.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gfsvpkvbx.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gkvqjrzjw.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gnxwooshz.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gsthqkfzg.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gpnoavlzk.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/giimnvjho.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gheengutl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/glourcoci.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gtnsbaebp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gqukkkglg.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gudaixjvj.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gygmvlntk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gzagruzwr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/gozwzfkdj.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/grqktpzok.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/goiapdxzq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/ggzymljpe.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gwffwunks.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gnpyycexy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gnhucvfom.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gvwfyzvdr.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gcyavztaj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/givzmvjmb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gwpqocovz.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gtriiytoh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gruzqgtod.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gfxodiwgs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gcqbqiewp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/ghhcfikah.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gsjupegwq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gqbhiapkl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gtoajxmdk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gzbahtzqp.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gttshslvr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/glyemepqb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gexsucbvq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/glhvgpmnw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gprvcwvvy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/grprwlvvr.sHtML


<!-- 参考信息 -->