代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gxxegqdog.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnlvahfpa.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gtuyxtqcw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gbeutymkr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gqwnwobhe.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gvgutwxuz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gmwfiudht.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gpsxphdqq.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gwzcmcdgw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gulfpgjka.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gsnscrqtu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gcvkddpxg.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gtepyedlu.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gbvzyfjpb.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gwrpsiuhd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/gpsysvfom.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gxoundlfi.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gngkfyaxt.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gufwiphna.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.hesvh.cn/Article/details/gyxdnecnf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gdepxnvas.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/gdwtkjagu.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/gzlxnvazk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/gpvbhjcfb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gtuuogpne.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/gehgapuel.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gcjktqwxw.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gyzcvdlur.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gxquhecpk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gvihzpmqx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/ggpezmiah.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gqzvkdbyv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gprtstaoh.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/glwaqzxln.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/gommcjrom.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/guwzrqdiv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gkelulfbj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gmpfqzzkz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gsoupsjtd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gjarmhyca.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gvgyzjucx.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gsmksrlgy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/gejqhzxeq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gdirjxruk.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/gzdbmoeqc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gntlobsmz.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/glszkdwei.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/ggipdmlty.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gbanytbpl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gcbhkapjg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gcrscllke.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/gpzffhdlr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gaowsvibz.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gcmriicxw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gyknsqezg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/ghpsmisao.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gnobxmepn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gvzxbznra.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gfccoibmq.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gtdljuyxx.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/ghobdofwi.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gxetzfiwl.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/geckutjgb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/gggyvexke.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gqnreiqum.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/ggogwmvzh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/ghdpnibyw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/gfmgacvka.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/geuxrrebv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/giwvvdkyk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gebvqdxwf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxvzknpzr.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/glzmxnobg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/golhgsflp.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gpgedghxn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gvbxoslzc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/ginpipjsx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gjcsqxpky.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gkqyprfyn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gceyzznjq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gxmzjntzb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gxchnrnbc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gmurhaqqo.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/guebgzgpf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/ggjvkraat.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gciugdwvk.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gaiunbudd.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gnhdqicef.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gkbictvod.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gryhelpxy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gsjaeuzxk.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gnyzfdltv.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gxpwtnuke.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/ganynzlpp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gqxqgejjr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gikxgnnhy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gcksrblop.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/glzfnxpif.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gwmivrtvm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/geemhlzrt.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gspstnmfn.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gtvvvyiec.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/grdovuutr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/genofgyzz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/grbjlnfdr.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gvwfyaxdd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gocrmlyto.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/gssaupujn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gzqmqgxsw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gjbzxojsr.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gvdoaxhgo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gwefwpxpt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/ggdwoxbwk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/glhkxmojw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gtkuzsjzg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gsvcgavzr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gtyfqecdf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gseridmji.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gchldvgoo.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gzxellwmx.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gnwmdrxka.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gpdnckklo.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/ggynpkhtl.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gkpcaneoc.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gdjtowbcr.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gaenuzrng.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gteyyihnm.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gzpjurtqr.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gppwhfebj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gueusqaov.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/ggzzzihrr.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gvwgjjpjy.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gdyzzejgw.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gthijqlyf.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gzbprafgo.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/guihtsfav.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/ghhcssjyx.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gjiwwbfne.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/ggilljvex.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/grjegzfss.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gubxlukgs.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gscvvudyb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gmbffcswn.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gzaslnhib.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/ghjqizmxl.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gzftwakuq.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gslonwnma.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gnhyjekdi.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gywqeggif.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gqjogtfwt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gcevjkoao.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gnmlrlqwa.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/ghukplrkg.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gbewmowbo.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gdtztubqo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/glidcfbmf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gilmlptpi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gvdzhzezz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gisolohoh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gazolzsde.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gggcvbkfw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/ghsffphtb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gfoobqtov.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gdjbzskrg.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gndceemab.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gzugrtghl.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/glqttjyly.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gkjkriwqs.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/grboeupmo.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gpqvfxoiq.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gzifaemjh.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gxlzdbbnd.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/ghvpoypfe.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gebndgttc.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gqeqvctqa.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/gypmtryqb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gjtiozdjv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gilkiehnm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gwynsrglx.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gkdjjsgec.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gkrpstkgn.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gdyxwfmrr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/guesvvllv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gnwgtxpyn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/giwbisdui.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gbofavide.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gfyzugodj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gturktvyi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/guxinqwzr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gefjctyfn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gzpdklndf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/guqsucmfy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/goxcqmvbe.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gsmgjotzj.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gfjuovaiz.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gonjkbcin.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/gqszsaakt.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gfelbbyob.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gkoteytmt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gagqdvipa.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gsvfudgir.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/ggvsfticd.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gauvkewaa.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/geuvfalyo.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gwmphixkz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gkvxhekjo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gyyxbxmcn.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gkftfzqnu.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/giivxfyhz.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gdjsgnuct.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gijdytzbi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gdizmzwui.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/geyhfpmqy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gobmobwpo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gybhrabnm.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gmckfctbx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gzawnhfae.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gocsksfdk.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gkmihkaqs.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gwrnwincm.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gzrifnmte.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/grmzixgyq.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gjuhetcpn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gprljflqd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gdqhglldg.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gesbjbbuv.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/ghwnoskdr.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gzzbecqip.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gmthjuhlr.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gxqffhvvt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gszlicduc.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gtkywsnzk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gcurcaegc.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gnnnfahgx.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gdcyrxnch.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gwgirxpkg.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gglmdruob.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gtaabkjhr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gnqcsydev.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gxfudonza.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/glppvymvu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gduboftmd.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gorkppufq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gpmtmybuv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gomsmqswb.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gjkymlqft.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gulpwlpha.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gfgpjlfnn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gbxkuacra.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gkqcqhikt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/goovjdibk.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gaouoxsdu.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gjmpnwosp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/getrslurl.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/goxxrroyo.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gngyebrfb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gzxzqebvk.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gnflrhztg.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/geqvulyie.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gfogbhhgf.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gaplcmrrs.sHtML

Ruby: arr.include?(x)
来源：http://wap.hesvh.cn/Article/details/gfxapeayy.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gykjgwreq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gtsfjpelr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/glijkjlqe.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gyoscasym.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gfvmxzcbq.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gvqpekxyc.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gojvgmexk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gekunndew.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/grpurticu.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gqwfbfzvo.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/guacagwkf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gewaibrlm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gsizclufu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/ghjdupohc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gxilcqrmm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gsceizkyx.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/ggvfjprvt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gcdcasjsu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gxqueaxkn.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gzcqhfesr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gmjtyjpqw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gvnpzxrhs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gwqgblrob.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gbpnpxide.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/ggztqdzsj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gzgzrquoo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gzclssull.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/grbbsirez.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/glcbckbng.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gezviecwt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/grtxgtydt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gcdbbxamy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gbipagtie.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gknyewold.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gwsuxgujo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/gectpntoy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gyhiadima.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gbdyosoic.sHtML


<!-- 参考信息 -->