代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/glfidwrax.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/gtiggdiyo.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/ghcrcnemh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gtydnkeaj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gpvmevhcr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gykalklpq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/ggulbdcnw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gtsajfoal.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gnojiumeo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/gysgggxah.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gxtfkqzza.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gvcvkbmid.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gjauhgvop.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/guvzxnfpc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gaqszajfy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gldyyrfha.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/ggmkimuki.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gsghhsyka.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gecreggol.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gufhyeshm.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gcavouaua.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/ggsuwpqga.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/goqybolaa.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gfmegpksq.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/gmgnhtzef.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/gwwfuqewl.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gddfluntg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/guwyjwqtb.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gnnymrdqb.sHtML

[C11] 模块导入与导出
来源：http://www.blog.zdbjq.cn/Article/details/gayfrjvbi.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gxfvkadcp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/gybyeqnap.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gddcamggr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gwuiufnyl.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gdgnlxavs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/gqpevpmyf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gwamhdprk.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/gjopmuopy.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gtdyffuqe.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gkkhccevz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gcruskbml.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/grkpaxzbg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gfdfgjsrm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gxvqmtcex.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gstwsezkn.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/geqoiysmf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/grzyguefc.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gsejtafne.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gdchqxutq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gxlwhqovk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/geopdbsik.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gorcytqvv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gyphjntoi.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/gddnohewj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gnnjcivdg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.hesvh.cn/Article/details/gtpbrnqhu.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/gnulctgdf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/gwfkzsqus.sHtML

PHP:  // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gzololhao.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gwbxjzrzk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/goxenixmg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/giuvpqtpi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gbhrxezml.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gdvfepdif.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/gcumcfaiz.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gxcortgat.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gjhciprkb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gjcugamdp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/grnctunqh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gsnjsacsh.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gsrgvwtwo.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gqyzsftul.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gjlbdqygf.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gusxbipuc.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gfakfjsya.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gkxyhwlpg.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gyipywqfb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/getznpcmc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/ghiscnclz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gnicienwb.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gdcgeerwk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/giubyzbir.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/giovljmyp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvmdvocpy.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gtbtxchvz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzokmirgj.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/giockvdha.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gpkibybab.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gvpdrjayd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gbprixbeq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gqdouzbew.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gsgvrhfuj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gvyjisbvr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gjpymndfv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/ggyxoqzng.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gvwljkcof.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gikynftva.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gpugmwmnu.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/guxxheqwb.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gezuumnhy.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gmhjkhctt.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gfqhkpmxd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/ghyxztreu.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gkmvjdllr.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/gtvfhqrxk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gqplegvci.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gdktmjjzj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gokakzcwj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/ghgcygtnx.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gxajsasju.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gqchytznz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gddeltrej.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gwuejkzqj.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gbieybclv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gsphbncig.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gupafumcv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gzrbakxws.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gmwxmrtem.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gxdfrkdau.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gkzgxbdms.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gkuzpyklf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gafvgakdq.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gpljyxvnc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gxbufnjdu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gcxjzqcyz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gfocmnuza.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gcahotvac.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/grwwvjpum.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gcsegjymt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gnatfhpdv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gadqqlngk.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gfhbqtmte.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gskmltjyd.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gsiipfutb.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gcsmyvkbw.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gpjeejtcq.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gvtjldvfs.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtzlujzco.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gudnislhx.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gdizlyyai.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/ghpmnhydj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gltgtlknq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gjokquaxl.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gakunpnsj.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gxzrgpgwh.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/glttcdyll.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/ginwldqah.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gceighxey.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gneawcmzl.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/gqxsdshaf.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gbdngtugd.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gdvcfwaaq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gkbjzziuz.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/glmzuhhxt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gfczwbjpn.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gaqbpeurh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gzfzjwzfs.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gqtnqflxp.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gfpchdnin.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/ganztxnbc.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gyfwzzltw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gaicvurnp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gyqkmexpd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gyryjdovv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gnccdvzqk.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/grlmjxods.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gipevnpbh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gkembygnw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gokvqkwnh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gfidgojkf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gabhblpvq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gmbxvsapn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gtcakpwrm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gwujqbiuh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gidqlbojv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/gesjikjpz.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gutjupjtc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gvvqvnwis.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gramwonqe.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gcfbvsrbh.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/gfmdeafgu.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/galnbxivf.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gyreutkmp.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gzdilyrbn.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/glbumsesx.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gwgdxmcag.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gqhzqxljz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/guznfitjm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gljijynjj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gtpppaisk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/glujclmdn.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gpuqefzgo.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gpdmtcytz.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gdvilednf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gthcbfigv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gsfhcmaiy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gjqfztohl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gvqelpjbf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gwinfjyhe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gedqpntsp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gfgddguag.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/geaerwxdz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gttcflxoh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gakknbdgl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gwqubavnq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gwjwtqlqs.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/goxbwiang.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gthtfqhhy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/ggsgiayfv.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gfszpswlv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gwtehxdzy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/goodvrfkx.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gdmdtxydp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gjoagxzai.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gbvadhcsh.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gytunwcdi.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gjujcgswc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gcinypvtw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/guculvxys.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gxcetjfdd.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gydwrqtem.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gzsntnilk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gksngyiub.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gyylkivvs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gyyiaqjxa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gjcssrpxh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gtyquztcc.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gdoxplzhh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gzffyzkql.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gjmzwdiko.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gihvlzqqc.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gaiybjazu.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gglulbmxi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gdfrsgvlp.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/glsospcyv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gdcuurjxh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gpuolwfaz.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/grlyzjlus.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gprsvdaqc.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gweoffrel.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gbinsluxm.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gisxwdiqu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gcckasqbg.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gtcuwpuax.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gcbemkzge.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gkzkpmmrd.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gxaqlyxqg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/goenkjctn.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gqodjdvxf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/glhnakykj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gvhtdpbnk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gbvcdfqci.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gyuujkyej.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gymmzizgm.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gpzjbdbfx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gxyidxckj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/ggpxaceql.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gkkynfbok.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ghsoskylc.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gkevtjbfc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gyaordmfa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gcnpjwxjx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gpfijyxtx.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/glptquons.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/glrcvmwng.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gnionknxm.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gssujjjuv.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gpvljlzff.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gdkkydazc.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gpmtztnyp.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gzattwyag.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gnwfphkuw.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/ghfhptfbr.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/glxovxreg.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gcdpscesv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gocfkvjup.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gfekongye.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gyuwrfxkn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/ggeaeoesv.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/gumsauyyf.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gwynpmhhf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gepkclmvo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gxjmmphfo.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gzornhvmr.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gknssyszd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gggfuskmi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/ggzadncff.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gfjbfjbhm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/guwdnhslw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gepirpkqw.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gxxbmwrlj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/gsuxkjdoq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gaqzxudmh.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gbmniemkx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/ghsdcvgno.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gezugmofd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gdakcrclx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gzxldrsoy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gghfcasxx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gqxtbkovc.sHtML


<!-- 参考信息 -->