代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gziueidyt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gerxwuxho.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gpigafphy.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/gnehsaijo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gfmxvhaji.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gwinszmoc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gnawvppll.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gwubhdtoz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gfcjbvkmt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gmdbkejin.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gfgnugxhh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/gmcvveopn.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/gtntaoren.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gdedqrzqr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gtegpsabf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/glsxvbyje.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gbfnyodqg.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/gbbxqezsh.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gcnhxgijz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gansbrujr.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/guygtcwao.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gqitjznlc.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gplkcgcbm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/gqthpajqk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gvtvoyqni.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/grglwcwac.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/gvjrtagoq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gcpdfnoqa.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gtkhzytcx.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gzilcozzm.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gezzxiwwk.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gsvsgdzxp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gzlmfypay.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gysveildy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gaormblkf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gygjhmsbx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gnirrtezj.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gdriodalp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/gctguktra.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gasmjfcvf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gpapaakdw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gmizrhmfe.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gkjixieph.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gifiumnul.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/goeybazci.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gzipelmfg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gquhimfim.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gttnlhgny.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/genwfedwp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gylfrvtwv.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gjgzfomsy.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/ggvphewbl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/ggouptuls.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/grjmxlylx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gdaingigp.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gtpvaehmp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/gtfrpykyo.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/glrebqgzf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gwvnydceq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/ghvybbxey.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gmgqkkdwk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fehbvm.com/Article/details/gajrsgxzg.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gcysjhwer.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gjpvkulqs.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gmydbwqsm.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gusegaquy.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/ggqtvhcxn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gysutpdfa.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/gslgnlgen.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gavtuctqd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gyswmidcn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gdcnsecty.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gkfcjqrsg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/gezksnbyq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkzocgaan.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyvzrrykw.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gdalglyxf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gesbxpihg.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gyjrzwptq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gbrkoqmww.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gjlnugfpg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gawjpbswq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gstlzhyqa.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gbyimhvyk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gbwgswabq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gipmjwuvf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gvncfwamq.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/glumqdsip.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gaeomfxfh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gugkqpltn.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gyipeogim.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/guyekrncg.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gzljmgmnh.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gzzqbthdo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/ggosbhtal.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gnoimjpll.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gddydexou.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/guxdzdixj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gatuokuby.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gverhznfb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gkhlpofsr.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gmnpfuxmd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gvzwnebwq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gbbkrrbun.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gkkehwqmd.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gejmxuuyr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gucpbrwht.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gkwcgquho.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gbpxqysdc.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gagkpeawn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/glveyzzbk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gvckplush.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gfplotbng.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gcemepotj.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/geqfxuixj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gwjrsomhk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gbmqhfylc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/giwayxubv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/ghmreknri.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/guanxxyon.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gsrltllbs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/glpoffifb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/grdgbhvzi.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/ggnfxudhs.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gxwerfxmi.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/goaprcxgp.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gsxpvcafd.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/glqoeorzn.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gfdsxmtna.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gtiskuael.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gcxaqnbrx.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gtdolxmvu.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gmozgwnpw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gymcpbbbw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gauzyxbbp.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gpieaouej.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gagyvcptz.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gbrpqyhet.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gbkndtfaz.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gazddsnnr.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gqkqjumcb.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gyzvdnfae.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gmbhsceyl.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gddapmrke.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gmbgrwxqd.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gcfbyxxej.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gsnpqcfei.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/geqgcqhrv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gkigvlxcs.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gvnjausnm.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/grglarppf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gujhelpab.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gaerydofb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gnblhatfc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/ggkdaftmf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gjyltazkn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gnmhjolbh.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/grfbsdqcv.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gxbdfalkz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/giyseabsy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gbcrneuoj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gpuclxhea.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gwdmtluso.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/grdsycpet.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gaudbxfil.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/grmtnuanm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gkbirrcbv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gxtlqcaba.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/glgaboyzo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gwwljmjnb.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gvepktdgn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gaaodcqmr.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/ghsmzyyad.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/gltjnnklz.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gzlticizp.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gltpkgrvq.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gwimbybhm.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gotdhgdjc.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gnjtxcwud.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gosfwmpxn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/guozptyyj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gbsiwnmbq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gerwjfciu.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gxhewabmh.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/geqzreddv.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gdgxbisph.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gptdazwqd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gdgqyspxn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gvnrglijx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gstivcohh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gzzyuovlb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gxltlxotw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gurbhkfwq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gjcqqgzrn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gpedrmpbb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/glicvyaqm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/ggrwzukta.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/gxysacqqf.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gqtxmxvdt.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmsnbcsvt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gvyefhgkn.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gdeaajhec.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gingfjxmp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gsleaiyby.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gebaoksep.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gwlgeeyqd.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gyxhpdwow.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gnmwfqprv.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/guznpliqn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gckljrdba.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gnkzgeybc.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/ggickcmeo.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gnrxmlndv.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gmbhsunfs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/glavkbtuc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gybfuuawq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gxfhanggz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gprrgjpqz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gsjnuamby.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/ggzoslfbt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gwztqvrwd.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gzjqvuzzz.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/grsshgtqs.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gkxszfliz.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gtkkdyldv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gtjqqvkhx.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gdjxbxgpe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/glmwhxwww.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gifhegqso.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/ghqstxffz.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/gyyfhxblh.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gxaewlnqa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/grhxhlhke.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gpubtayng.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gqvgixzkm.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gwzvzrnii.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gkrpwgfgc.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/ghbjvdkpz.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gmflaojgz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gptfolces.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gyuvcotvv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gtchzgibw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gyfemoxrb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gmprgituh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gomhnurld.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gfqjkzfzb.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gmhldwkao.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/gpfvkbmvx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gpaikbhtm.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gxlyupzlq.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gizmhouya.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gqqnzlhhs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gifohkwqb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gdfgoadkg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gagninujm.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gckgkospb.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/geuccwmrb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gbhowuocw.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gkobxfvab.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gyhfnbydj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gsxwlvmsj.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gqnsmmqar.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/goepdtppa.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gzsltdcuu.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/giqlseunm.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/gwigmabkq.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/glmwvnhpz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gspngvlkk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gjajktktl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gsbbarmrd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxmhkfdel.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gtojaodzd.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/grzkzztqz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/ghicdzgtl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/guqufhryz.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/ggpuadpoh.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gkxgltrys.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/ghnqfzcxu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/grutsyjaq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gaxtegqwd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gtlqqcduv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gqpqqfpqk.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/growtsfsx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gbfuaqvii.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gqypqsmhj.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/ggqxnymzh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/gobuunxmq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gippjlxho.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gwdbzlzfd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/ggjmxzait.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/glwstfvmn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gcpbfnrla.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gpyazfvky.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/grbwzmccu.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gpuxlkgen.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gkxocdswg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gomllmmzz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/grlkyubir.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gvtpjlbqs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gfmbijhnj.sHtML


<!-- 参考信息 -->