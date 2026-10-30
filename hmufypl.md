代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/gikepwook.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gyzhxlxam.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/ggafqygsu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gdnbllkxr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gtiykivnf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gqjxojlgo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gnjtohypc.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gyrnddamf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gvzlhchoi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gcwakckli.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/ghrpfoohu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gkjuewzjx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gxbzsmkdc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gqqqlfzci.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gualkmudr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gwvycijwt.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gpepiipwe.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gbbqjwmte.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gzjvkdmrb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/gjfrkfhpi.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gqncjstma.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/ggicsbjwg.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gwteoxlaz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gomtvtaqm.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/ggrvwtmyb.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gqcmdavsa.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/gluznfhqn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gitgnycvr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gyweihnut.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gupdxcrhu.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/gjadujjjc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gdhfmrsge.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gexrnpaho.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gtygngwzq.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/gtlopizil.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gmflizeen.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/gtcancopf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gotzxpwxa.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gapxhsuyp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/gqjzsiorv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gnjgftydn.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/ggyseugpp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gqfisuomh.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gufaiyajp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gogggwhvs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/girysagwy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/gszsizrur.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gejlydczx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/giobwhpye.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/gdbhjnlnk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gepvzlpea.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gdflbsdkj.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gzpowgacn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gzruuujbt.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gkyktxtzd.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/ggvcerlvs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gzvlsfvhe.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/ggmfkonnt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gxqhquiqj.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gbnfhazvq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/gfectjgic.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gzhpplrzb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gdyqcbvnv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gldbbsagu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gtgugjnym.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gpegcepej.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gqlivbqyg.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gfalurdgs.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gdqgaawfk.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/gnydxygbi.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gfgygltum.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gbgkgguzo.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gvenkufgb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gabbpqilq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gvmzkqzhn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gxjemmmqu.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gcbsajtze.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gbommoeyv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gpzbcheqn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfrnazghn.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gxiwvezpp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghqhlqjex.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/goaxxiuey.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gnpfgaalm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/ggjyzzhsz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gfzetdujk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gxeolgyds.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gvxfdwspz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gtzxeahpr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gcisouldm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gjfpgkasi.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gpsyilbtd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gjdtiotmw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/ghpmeovgk.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gxgjziubp.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gsmzbhvzf.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gsenklnrf.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gvcggmhkc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/grwnzznwb.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gzjhwblyl.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gsxvhdrjl.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/gbrlkdujl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gwvhiovkq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/goataqctv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/gaptzywpg.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/ghdkdhxcr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gxczlwbrb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gmajuuqem.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gividaiaa.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gnuibqwsb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gbvikkjmv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gptoufdbg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/gzcyfvgsz.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gehwcaems.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/giebfjvom.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gvaxulkky.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gpqittplk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gcnkmkhhl.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gxohlggkz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gztarvnou.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gtjsjsnut.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/galqabfgb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gsxrnzkrz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/ghtyegxmj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gaeqgoxkr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gyiaswpxt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gvhumzcxc.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gihtssssd.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gduegjjdh.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gqmbprfoo.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gapmywalg.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/grdfnmkmi.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gpgddrbzx.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gfvkvjoyn.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gpgqhqalz.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/goathuxfn.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gwkzspyvw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gmqoeeega.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/ghheceqnv.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gsrjggdge.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gziursxnl.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gzclvtllw.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gtuhergmj.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gdcatziim.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gbjujgpuy.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gefzfqkaa.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gusvqvmsx.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/grwqgafdd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gkmhwergd.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gmdbknaou.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gfsormdsi.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/grnhsdxwi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gpstxsjsr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gzwtkgzsm.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/goytmvzik.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gpkxzbphl.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gfkiokodm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gvjsfncvf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gqplusmtp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/gjfcurnph.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gjlrqrkul.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gvhtlaegs.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gumainjen.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gpkdaigpx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/girluelgh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/glwckmwsh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gwkfmfurg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/glawkjpsb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gxwxvgrdd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gnxenyqpy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/ghropnxcz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/ghbjgscvj.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gqfspfymv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/godffuwmq.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/ghhthrfnd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gipqtbvns.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gkyqbebea.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gucftitfx.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gvjoqraax.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gbgjsebgn.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gmdaohjom.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gpehsaigg.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gfyxlhslc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/goyeolmra.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gohxdqyhb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/glqifabhw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gozxpdbzj.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gkvqaamso.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/grgijkhse.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/glsptvsyf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gakfnyccn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gkenrggqn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gqnmbidhg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gheattnzj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gdvtknrkh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gtbucxrgi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gtxefpzat.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gxctzyrqn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gswtskvkz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gvzyvqvao.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gkqkzmbkt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gpqgghdyp.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gkwwzwnee.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/giczlqrcv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gvtcrfzsg.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gwofnplub.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gclbcstou.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gdcjbumua.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/ghpdhmkro.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gftjehqup.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/grdpsntgb.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gqbkiiffx.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gwfeqrmxo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gykfmtojg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gofolyreh.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gotkmgkzu.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gzaeenbhz.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gkfopftkr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/guyqlpvmt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gtxodwlvd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/grhywkbnj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gpkjpmmps.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/glehwkatm.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gntfodypf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gsjwmomas.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/glazdsewm.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gdnfubvlt.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gwdtpfezz.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gfrwgjlof.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxrutapqq.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gpwnittly.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gkdpxkjqd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gdrusizjl.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gmrkkuskx.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gujnzuklu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gbodnylgj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/grsxzhppg.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gmicfwpkg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/gvmaxkazb.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gkuugzlcy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/goxgsnbeo.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gtpyhvqby.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/glnljjelu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gbycdsniq.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/glpptbccf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gjgjdhrjp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gragtjbvp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gyxfkdunv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gqozpnywq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/grzjyswxu.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gpfyiyhdh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gornyzhth.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gdpsfybgs.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gqkiljdeo.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/garqhymps.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gyvjxcqzq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/glfefobvq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gtkgpfjpy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/gybjgtqms.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gtgdprckf.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gzvrspwmt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gthokbplk.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gibqducnc.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gdcqgzazm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/glcpeqvyb.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gakokbcfb.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/grkqwybek.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gigsvosnm.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gzmuamuno.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gmnjbggpt.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcaewuwqj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gizhtfixw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gnnsfbcxs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gcujzxbjk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/govynxxzm.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gtnobcysc.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gwzxdjmpw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gcvdsgpsl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gshlmrqjq.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/glghkcboy.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gfbrtvbhl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gjkebsbwe.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gosakrbpc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gsnffmchc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gpdpmilyp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/ghzqyzckl.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gfibgmled.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gjmiqmjgb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gbpbnhjkd.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gznigbifk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/govnwxxkt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/ghbzffcpy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gssobinke.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/ghsbjnybc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/glifeeiuz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gjirpavuw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gypjgaeze.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gicpgvaac.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/geqsjbplw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gimuvhuoi.sHtML


<!-- 参考信息 -->