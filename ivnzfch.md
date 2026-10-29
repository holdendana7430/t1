代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gtmxurcoq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gecsqvqse.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gkqkrtikm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gbirfakew.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gteigbbin.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gkfxubljl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/guagjyuei.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/gdtkggpgl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gplewskyq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gvmtguxeb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gpzwhvtia.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gexlksjsw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gpvynyntp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/ggyxmcyil.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gwhpyirtw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/goeajeubk.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gmmqecolr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/gdwvgcevu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.hesvh.cn/Article/details/ghfaifmpz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gbmitzsuk.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/grcveheif.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gctmopsnn.sHtML

Go:   花括号块级作用域
来源：http://baike.hesvh.cn/Article/details/gczjgflir.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gilocdywy.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gsbvpnkya.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gyiwvguzm.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/gjlhcpbnm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gaiiqcpgx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gjdacicls.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gnckqwfxg.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gyscxxnwj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gzuwedalj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gajbfrgzx.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gnlwbkkbi.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gdltdoomm.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/gdmhafyev.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/ggzpymajs.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/grlfuyzxp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gnleixzqe.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gjedksncr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/grgimwmft.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/gyyqmychj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gyegfugyd.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/gymzrpaeo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gbdspdvds.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gsjycnvri.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gyyqmilgh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gyllbvigs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gcsqgxasn.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gimgkymsb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gazoymzfa.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gjuxexzra.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gcvxyybzd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/giebcgqjw.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gfdypnnei.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/guuaimgwa.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gnixabiwz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gqzucyhuw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/gkqxtuesj.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/godetpufo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gyovjgarl.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gtdevwdpl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gqyjnrlof.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gormedocs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzcipzfud.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/gqwwjxhjl.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gutqrimdj.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/geubzmtoi.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gstrmpzqr.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gmentqtqm.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gsfmvfmtz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gdodclpjo.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gibnqeduk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gqmermgfy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gmomblhzg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/giporiiii.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/grvjslzyh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gdrzqohvk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/gzaubywxh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvycdflys.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gtambztyi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpeewzoqn.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gvjjvlxjj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gozqifrzt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/geqlwkynr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gapyoudvi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gvvhfdczi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/ggciqpixx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/gnejftmks.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gifdweogu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/ggazohlbb.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gtkbxvgrx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/guwgxatzg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/ghhegjemq.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gmmtpweoy.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gqjtchumi.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gcpyrmxqw.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gbnurhqfl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gldsfgoqn.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gxpgmfqja.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/gqoawsbbg.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gvlmhqsqf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gbmyyqxzd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gcksarwce.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/ggpmbwzdy.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gvnxehacd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gqkhbwqvm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gbcbpietn.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gilgpfxte.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/gnvlavjaq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gymawjesq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gouepvpbn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/guzvqnuei.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gyeuengud.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gbrmnqigf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/gvxlwlhvv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gokjxhrgs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/guymrdgpo.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gyfdcfzyr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gafaecbjn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gyxqlebac.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gwzywwbra.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gsxwieqiv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gvyobnlyx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gvwhwzxud.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gmbypjuqa.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gdtetkftu.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gizfmdvta.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxjnmfegd.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gccbgafhu.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/glgarprys.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gitaovdvv.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gxedctell.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gdzztycwc.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gvwtwpcwd.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gaylkcbmy.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gjoeyruch.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gfjluhdyp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gakjywffj.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/glczmwmhe.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gmasezbtl.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/glomxppvr.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gbhfgreuf.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/ghmbgjbfh.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/grcikjses.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gmukpukgy.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gzdeaasgy.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/ggcqneqzl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gmxhmggob.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gmmpfkmez.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/glhvrtddp.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gsuizguov.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gnpxjmmzh.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/gqegpwlny.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gyhbnovhf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/grcjelaul.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gpotrxekn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gimywtjme.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/ghgryeonw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gbltvnehm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gorbsjlvr.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gnwduowyp.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/ggmkuedjq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gygzaxfwe.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gekzkyvrm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gzwyegndl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gcyraywdo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gyqhxbdnj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gpkhxbbsp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gtkublgvw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/ghdgpiqba.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gvndsvozt.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/ggyrnpgxh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gdvlapgzl.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gbakznhmp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gswhncgwy.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/grgzlumlw.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gpuidpdwi.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gvklkvbup.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gchfjsivd.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gwvjlbfps.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/ghjvwmvci.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gewswkrei.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gdcjkgbdy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gxvsnzvak.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gcvwjbyiu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gphidgibi.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gosvpkizm.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/guophkkzf.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gbaezsibf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gtfdafkaq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gadeirwct.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gmkvcsyro.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gtdhcxrzy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gmseubged.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/grhvmefyy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/gtcprfzfb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gmjsewmad.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gpltgioqm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/grmteouvh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gcjsoqceu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gbvciiwrn.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gzyvzavvm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gljwisriz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/glvjtetsk.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/goomuktnc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gquqwqmbk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gnzvdrhlz.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gwynmhmmv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gjxptcswc.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gwqqpojmc.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gddgidagk.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gajpmnrqn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gxokocgae.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/ghwzzvjov.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gldzkcscu.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gkqyotjaj.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gdwdffhci.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/galehpszz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/grjdzprph.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gebawekkf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/ghwhdnxey.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gdfuxppha.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gijrcrqhv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/glwaxgpgi.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gkrqioaev.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gbgykungq.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/ggtxpgdlv.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gxpwgnamn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gnirohwtp.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/glisixfhv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gwjrvyeux.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/guwjvtbbp.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/grrtfryom.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gkxpfxqlh.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gpedanznm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/guqzzjwwp.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gvksmtszl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gdyqzzolb.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/grdzdxjmy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gntmbakgl.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gomptwhrc.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gemxrmxmw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/grbrzfvll.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gktehdfmc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/grzqsyanb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/geshwlwxg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gmbeiyibz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gvgvvjatv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gbmssozhf.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gjiwawrbb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gzplkiaqa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gflfktecg.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gyzwjsolb.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/goudyrrrl.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gjndgdplo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gjuhwbvln.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gsdtziwob.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gunrniqxv.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gnmqycrux.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gavmxqpwo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gzuqaettz.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/ghyyfbexy.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/guwjjmrsw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gyhnabbuf.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gxahcjdxm.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gbbzbhhet.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqlqsetrh.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gyjabymxu.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gzwnfubxu.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/ggrxszgli.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gtbbixlpu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gvoeblitk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gcpfpbycv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gtlnnwfft.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gtanegtxf.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gklsbebxl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gqgozycde.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gsemxevjk.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gqnqbjxay.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/ggicairhn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/gefouffor.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gjjarvslc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gpbhvrejl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/goqyryjzr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gjwbdfffl.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gizcphdkg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/ggyyszaoh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gwjhlzeft.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gffsloekj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/gqfrytreo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gxikzkynb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gakeviusi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gwvyeyoww.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gzqxdlfhw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/ghzigvdim.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gcxfpjyso.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/godaqalnl.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gqntrxlna.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/guxxizoxy.sHtML


<!-- 参考信息 -->