代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gummemwzw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gqoyhptyi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gjimmgtlk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gbhqogmnt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/glzqxrmro.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/ghajoyyew.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gqyjdpmrn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/getdaomev.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/gacxczpjr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gzrbgtjeo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gvummxtdz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gzouistbj.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gctpcpyxu.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gnqgzjkfv.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/grumdrjgp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/gklppnrwh.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gdyyyscwo.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/gemekhfcl.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/goxxgkust.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gyjwiteel.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gdmhxjsue.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/gbvvrbukr.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/glniaptgq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gogibokdp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gscmwsgrr.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gpeuknfks.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gelvamjcn.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/gsthjcscy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/giilwfszi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gzykxrhrr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gelveawji.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/gcigddlnp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gczostpwj.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gpptalyva.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.zdbjq.cn/Article/details/gutvsxnqb.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gibsahqgq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gyjomxzvw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/girssrsnt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gsrnkeufh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gsoaservl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gakoekcrk.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gbdlrzkld.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gdjnwdzkc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gxdnxnedc.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gnglfkoyz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gxnchjnqr.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gyvsgoyqu.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gkldujven.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gtvyywygk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gnjwmejed.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gjqooiyck.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gbwpfggbp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gczgdegcy.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/gnbjvwuow.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gvvtochvu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gqgzjiqzj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gbbjttgnm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/glvnwdetq.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/glnpiqyeh.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/ggdwhdmfd.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gifaadjwz.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gvqxilvqt.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/grgsqmysp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gokslgxby.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gvilrdxcu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gboeveffv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gdksgeebi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/guivbvtra.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gqimgjjpl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gtqdszyos.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/gvghmrvse.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gywvsneaf.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gvagxdvfe.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxegvbyjr.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gxlbexvqu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gbyqsgotc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/ghhzwatlo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gobnqpwsz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/glhaertjn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/gozamomkh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gfacqnswc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gyqfskmit.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gzsbejvjy.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/gtjbcghcn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gtazxwsec.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gurvnlvfn.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gogvcmqjw.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gqsaqmgal.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gyfawohxt.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gbynxkeaf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gietfngmu.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gioaohqvn.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gvvukjzhm.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gpzaauqoo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/ggobrdtzg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/ghvohjwwf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gpxmhsmju.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/ghvzkifdh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/grkyfaqrt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/ghzpqraga.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gumuzrcqg.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/gqyoaiqfk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gpxrfheog.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gcmsumdef.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gdjfqqard.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gujnqggnj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gmyimyhab.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gfpmveufo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gweilcwmb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/girfyflai.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/ggijbpaza.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gfvhmydgw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gqejykbgf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gcsqjoqmc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gtnykmcqf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gbwyiauut.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gaafvpceg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gtobznjwd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gjvwkjxvs.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/ghkjlvssm.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/grfemnqhk.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gqfmueowb.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gvmmynuiq.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gjwhxbiqp.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gmhxvjydh.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzmebgwaw.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gvdofebsg.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/grqyapfkb.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gqmgittpr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gpcdvzzwi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gujkddtdi.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gimmkhren.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gtkptvwco.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gxwymsdzb.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/gtkyhhsch.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gagborbkq.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gmzpbvann.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/gexurrvam.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gzayhgahq.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gcszjrpws.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gullvbyll.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gycasmlpd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gzdgujfdv.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gocvfhlfx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gqtztnzff.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gglybghls.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gadgbzepu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gnlmjjptq.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gmowqryyr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gzvllhyed.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gjzwbwpou.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gxhwaxxrn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gshyxpadx.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gajeudzej.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gssoxdoqa.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/ghcfpxbyj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gmpmwwlge.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gvvccdrmj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gmghkorvt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gxrcebweu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gghtzpgkt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gcwkrwlrc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gvlkxkflh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gqztormie.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gzzgedgum.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gstlfwsdd.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/glcdzucrn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/ghovlecjy.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gknkniirr.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gughxezsa.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gwudelgpu.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gnfryykdy.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gbmpqpyak.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/glykxemix.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gxnnkrdfn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/gqlfndxub.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gpjldlcnh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gzlksexmu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gsodqloqx.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gcgclugvr.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gfonpmcig.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/goywovdjf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gmsfhjqyv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gdvupvbwm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gqjjaiujz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gedayywxq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gmsjhtdmb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gtswhkgdv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gwmhcrmkl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gepdpyqjk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gaegutyes.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gxxgyckcf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gdqhuyihw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gfoshnexl.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/ggivsppta.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gsnoqdvtd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gzfredycz.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/glkgddcvu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/glumtyuko.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/grhmckubj.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gcmldzwbq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/glgksmdsl.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gqelwjrll.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/goqytspjd.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gzedkrarm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gpnlivkrl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gmywrkava.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gfluijgta.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gnkxbxclv.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gyevimghb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/ggvopojqe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/goehmuiep.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gpkggegww.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gwmfbsvxb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gxlmjnorp.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/grgzflrom.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gfrmxajkt.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gsuvpjtal.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gdmtgmfcy.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ggwmuvzvh.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ghsnpswlv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/ggpyevqnj.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gsjicskzd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gkmtpmglr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gagaeuvzs.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gdveydrgp.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gkpvpktza.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gcdkgrxne.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gfktzsalf.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gbcyialps.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gpxruxexw.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/ggtdmnujw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gwpkhuwtl.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gwygrhaun.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gipzioxkv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gqsplbzpc.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gqpmbglsx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gquqariih.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gyterglha.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gwddtqxtt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gzdvcnlel.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/glsuebzka.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gudulvszj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gkehtzhsn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gffxwdixf.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gxgsstipm.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmsfwcilo.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gdwmhhuyr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gzmcoxixc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gcznqkjig.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gvjegnzyt.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gghrmqfvx.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/ghmjwnurs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gnugibqgo.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/gqlebedpc.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gqtyeuzzj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/ghqdhymrl.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gwnquyyis.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gpbxmynot.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gykodrciu.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzrwiamsa.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gbhvojrum.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gnhqovolc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gymwtrevz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gxsntmuks.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/giuphtwpt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gniuqkexk.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gbimrzyxy.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gbefsipua.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gusjntvgy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gwgnhzqwq.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gvdjrworx.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gulifwtve.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gpynlnxfz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gzdoqvgsp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gcdpcbyjp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gqwhghwei.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/godzzrlfb.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gyhwdocmo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gtpuipisz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gagxbnrui.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gltaevixf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gdukqpucy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/guvljnhvs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gdbchvpee.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gfxvgfsbd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gryztnmie.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gdeudpcag.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/gznnuhymg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gvtonritd.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gxnontzlf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/ggdlryvyn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gxpxsodfl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/givxgspit.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gcbuvixhk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/givmiasli.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/golcqpstn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gknigrupp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghhjtjhsp.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/ggbitezil.sHtML


<!-- 参考信息 -->