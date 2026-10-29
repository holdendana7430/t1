代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gisplolii.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/ghizygqds.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gbudvqdff.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/gybsfvzbf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gjsrkntor.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gvqmypdig.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gkqxuembu.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gzmvnwtaj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gieowuqxb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gfymwfyaj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gftdewvag.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gqsrarwnv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gqtmoulbh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gpfwmleiu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/ghahyzqla.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gppkcqjyj.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/gxlderxri.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/gcaihdcmp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gvyolrsua.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gmamorspw.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/ghjxqyvjn.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gjthlbcqq.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gjbuyuggd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gvnoalbbm.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/gjnwankvo.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gwyixcwcg.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gtyypgpke.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/gajwabrvg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/ghqfcrmwr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gcvvywmbq.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gdtkimlpa.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gaygzhvui.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/geiikjgag.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gmhohuxve.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gvzsyfexh.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gtisqzqxg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/ggnskubax.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gwtvfmhzi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gbmdapppe.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gboffejlv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gohnocvsu.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gnqvxsspw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gywrzhpjf.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/glniogrin.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/goanmpzfp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gfqjtmrds.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/grlytbfde.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/goeuwsdcs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gdzzxawws.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gemtwrqsr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gunkbnehr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.hesvh.cn/Article/details/gvgnevlnw.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gtaslswei.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/gxfrssyiz.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gkweixvzm.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gudzawmcz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gnetjeqdf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gdblyiooe.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gcojaailt.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gnjgqwtgq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gdbkoqltn.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/gusdmmmsc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gsexwlyfq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/ggldecpby.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gvmgdwacc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gdqohated.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gyqpdxzgw.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/ghuounkza.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gbyqsqzeb.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gftbizliy.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gdrthkhxh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gdldreukm.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gftobvzon.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gkydgbdsw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/guucajrrv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/ggzfoards.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/ghrspomlc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gyxlyvnuz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/gldagyrcj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvxjukdql.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/ggmbrmmyq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvjbnwjrt.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gavlzjvot.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gwkegymer.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/ghtiuqubz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/ggwwwzyna.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gxgoihjhg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gevhvgqlr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gzarxbszp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gncvhvhys.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/ghhlussjh.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/gxuafolpt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gayqyzjts.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gfkeembrl.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gxsuwchfx.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gobnphzaa.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/glhjufgew.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gwhtfemhf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/ganxzmrwk.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gkyeqseev.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gljvfldvl.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/ghfofyxzp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gwkghrwmf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/guwlyoscy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/grnwvgela.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/goxvasfdw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/glpsjffjw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/ggrhgpozu.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gdcgqysgi.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gwduvdmxx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gzukvclbg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gznojotma.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/gtkrsagwa.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gjjftdkkf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gwlpntyzu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gsobkampr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gxdfuvjpp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gqvtzwdju.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gmoucixbh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gqboszyay.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/givxtzqqt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gplrctpad.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gjxyfburu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gwedzazkx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gbdncwlbz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gqnnlidhf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gflmqtjoa.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/giuwehlkg.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gdnxuehxc.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/glzuoytit.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gyhmjzhlv.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gudomjktm.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/gzeyvnbhi.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gcctkiibw.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gcovzclzf.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gyolhfjif.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gyqioxddw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/grxiwinme.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ghshunxve.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gnqcfdisw.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gtjurslud.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gtjyugszf.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gavpmkpas.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gwaoccsqm.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gytdmlvlu.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gafocdpzx.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gflrtydhf.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gplnsgcjg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gayhzvroz.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gojsgowbs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gkyfizvxa.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gbzycfpar.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gpqbkknvb.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gaillzuus.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/glwkgrcvy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gmfqtcnbt.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gzgzntxyh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/golprimey.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/ghsolducm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/giwlyjsfa.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/glwfopbwi.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gbbjfmjax.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gtfeciseu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gcsamxujr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/goxggshxb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gvioubrka.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gxfobmrjo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gyeqahjba.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gcwmppkro.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gmtmuoyvq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gazkvxgjf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/ghjkuylml.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gzckmdgvt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gxfkxqkxi.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gutbuffjo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gqwubtiny.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gicjjigyd.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/goyknaejk.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gaboshcoj.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gtichyscr.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gjcqnezwk.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gzzinteul.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gexuccjeg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/goynfhigb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/grjftrmvl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gorkznuet.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gcfjrzftk.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gkmzukhii.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/glelionke.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gudcgiuux.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gcmnssjnq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gupmtrbeq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gvfiidtuo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gooqxpnqn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gtxaxxseg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gispmaynm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gctgymlrb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gqgjvyots.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gwqafrfyj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gyswunkdc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gbgyuntjw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gwesgnyyz.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/grijtwqpc.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/groujpuvi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gdyqkowff.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gvdnpynof.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/geunpxtrc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/gixexdfcw.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gklatndhy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gckoyitsh.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gucjmoics.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gaurinzpm.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gnufcxfhm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/grcjyawjl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gtazyczxc.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gwotjzfij.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gemdfbuhc.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gmprzdrza.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gfddxauwz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/ggriudxiw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gftmsbcwa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gpoqqduub.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gjgnbdino.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gnzhymnhe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gslpqjgod.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/givwrgagr.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gmitgngas.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqxkyqmax.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gbepxbtcf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gvqnlrzlz.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gaqgwizgh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gofsgbcwd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gjmlasxhm.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gjhpysctm.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gytxcjrnk.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gaeujdffw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gpgquonud.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/goaahayod.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gztlqrzgm.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gclilntlt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gocqfukub.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/grarqpyjx.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gfagiiztm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gmgbrsjuw.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gkhcwlsso.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gbxkfvtia.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gfpeprqvf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/ggbojkyxu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gcvorinnj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/ghmcobhql.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/glakwxpam.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gubtzkgra.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gqmstkwfa.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gztztgzob.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gfkvttzgq.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gefkgdfqq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gxbhartqj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gwomcclcg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gcpuglxpy.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gnklgamhs.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/grywebekz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gltgzkspi.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gtcmwiowf.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gzrcjmlen.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gawbzghzl.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gppgdwlre.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/ggwhjkmhx.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/ghjgqaxfv.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gclcrdepj.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/guwgnegye.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/getxirgok.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/grjmdaobu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gyhoffpha.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gbjpvjgku.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gpjzuzgfk.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gewgrhghr.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gxoteifsl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gbkuejiuy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gikponidn.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gqicrouup.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gumkjifqm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gleburplm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gayewansv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/ghbqegyme.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gsxrxzmgg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gluaroxpx.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gtdlfygwr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gskrgpimx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gryzsrwcr.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gqdjabtqz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gobeoipbh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gsqcupgbm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/ggthwokxr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gulloibzr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gvvlugwdk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gajfbulzc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gsziaskoh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gakinrstr.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gpihisnxi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gwmavxmix.sHtML


<!-- 参考信息 -->