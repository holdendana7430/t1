代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gbpxxucfw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gvgjnjxrs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gxfjtysjm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gkadejjvn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.zdbjq.cn/Article/details/ghzdmaips.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/gndopxnxp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gejrkeaqs.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gqlaerbdy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gytrebcni.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/gtlhorvaj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gpreizijp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gsntyknuc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gphggkirs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gllxuqkfj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/grgskqheh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gpsphkkrw.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/gtduvwzen.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gpzkgembn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gvusmetka.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gkgjimtlh.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gtvhpjjqk.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gookyseew.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gekvwumoy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gvulqfjrb.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/gazprxwxj.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/guudtlsrm.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gkgahbctc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gwdycmmae.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gfqywuhpt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/gdysjlbfr.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/grkitivdv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/gxfiiznhf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/galpgvwyl.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/glveyyyah.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gmtsjvbca.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gillcxsqi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gkmqvvhxi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gtandlovp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gjlbcpsdj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gkrtzbfwq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/gznwfgzjf.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/goroubapo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gcfajnblg.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gslfkhyfd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gfupetwqh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gfhcayrfh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/grxelaotx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gvxyplzqe.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/guyjvzbtz.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gubviugjd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/goauamsxr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gqdkvbvqn.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/ggemmxvqi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gbbduuavk.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gxyupaklx.sHtML

JS:   // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gtqhfsfnd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/gmbvjqqsh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gvghtayib.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/ggkioykpn.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/gerarmcwp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/glvwoondt.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gciqcyxzg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/ggppfxbzj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/guzddlzzd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gacmtsznx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gocirhdae.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gfeccecxg.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gmhqmmvwm.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gkqlhpsbb.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gbnnyfthb.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gkpvhekfg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gbablkdxx.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gjbenyyjy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gobeoipsl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gjqktwdum.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/grafshavc.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gbogzpdtj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/ggqgpvksc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gdkebfrwh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdcbqbdoc.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gduyhuxpb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkftsvasv.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gvgxonswv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gihxzglno.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/ggxswrrfj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/ghmzzvipr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gmciblhlj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gojefrkzd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/geoamcbnv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gnofmhetr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/giuhckror.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gdphcommb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/gqoyggjbq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gwlqmgcsr.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gufrmcwgx.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gsybcuxsn.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gvfthkcmk.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gycurqhdr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gdcswjwxs.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gqbggzarh.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gauzpkfaz.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gsidsplff.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gskegpzjj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gbjjizlte.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gtgkrywqn.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gimzxiplh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/giptxqnbg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/gmzqqzwwh.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gcuaaernd.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/guuplqswd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/gjwadcycg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gkjatpbla.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/glewgruai.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gzwhsmwcb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gypuufsau.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gsfphtloc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gngjhvkua.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/gxcrxagvq.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/goyawlsan.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gsynagaps.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gkxtaecac.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gbepxfsaa.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gdgtkkgyi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gieukfpzz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gbhqqvdsc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gjwpvhbax.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gmvbvnphp.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gvwtppzzx.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gljhnwfks.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gqusuanrg.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gajzuvsez.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/glwtlntuq.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gufbsbzim.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gksvulrxv.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/grcdgszgp.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gsllvojnd.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gvgcisamt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gpqzgabrs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gzvwwmxls.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gdiqmlfad.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gjsaktrbb.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gehuuyusw.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gmaimxpny.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gggvvvfjg.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gwsukmfyi.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gmqrexmoy.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gdqbmzxfm.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gqmkznvkl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/ggudynaqb.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gimindkbk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gptsawrww.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gifaxvwlu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/glvjqieyf.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gbqdcacmr.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/glodtwatr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gesvomnif.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gsahppwtp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gjxgwaare.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gpcvggvfc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/ghmpsnlhi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gcduozmgc.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gvleutkqy.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gkabmbzdp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gjmowbqts.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gpukzevdl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gfezsdqwo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gwtbbayvb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/godiupdqy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gqmddtjbn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gkkbjmpug.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gfdyxtztg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gaclksxjg.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gztznhqkw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gsdnauefe.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gupqtsnvf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/girwzogzq.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gsgsinlxb.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gnnnawxxi.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gsyjrvuyf.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gzgccblnc.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gmefkinfg.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gbftkvfkc.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/gepigcywo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gqfubjkju.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gddrcohbq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gssfecdhe.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gephkpugl.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/gqmpprjnh.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gwefysrvn.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gfsbagwxz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gibrxysbi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gbcfxxdvt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gqiwxxgnu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gtwwnotzo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gtyhusepo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gsjqiaosd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gxuhfdweb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gatismqqh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gbulssnut.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gqcfeoyif.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gqagaxiox.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gbbnkgrjk.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gdqwjxiyo.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/ghrhyvpgl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gllysjgdb.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gbrwdaqkb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gktrksebv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gngjgqyez.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gxntzwofv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gxjggmsht.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gyramrimg.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gbaeqdjfy.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gghqjjcbp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gkykcdbsk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gzfochori.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gowhvurpg.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/ghvbndvhn.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gjnuhpwgf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/grvjwywwv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gynvubwte.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gxpiutlfl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/ghjmgtwec.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gwmvymepy.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gowtesrwi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gfxzbgjus.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/ggspgofgr.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gqjnxrzkw.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gzxgcbtsl.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gciynwfit.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gzvmqpmhi.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gsubkzogt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gnztoaurv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gynvbmxpu.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gvuelvuol.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/gyvtnshtf.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gmvhzejgi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gbpcxfmtr.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gfdnugjxd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gxizdzxjy.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gbqpbnggj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gtoxsqklu.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gptbwpwjj.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gfagqzron.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gpctzgtgt.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gbjpoxhjq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gdstewrgt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gzxptnpjo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gasaqgsmr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gofrlgmpf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gslprlrhy.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gaywwzfne.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/guotxxieq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gazbnywcv.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gcxuzzrwe.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gcxpoidza.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gynfdqtrv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gwaqnimoi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gqwitdmpm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/gcwcxvlui.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gtbqmokaf.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gqqxdtpmb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gxiviroxa.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/gyyajceiv.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gxwlqjvpp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gjqrxjlbm.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gltnlfcua.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gsrephlgt.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gxmapecor.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gpcvtkeul.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gndquojsy.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gyjubdqhh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gzflhvnqk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gpyfepxlb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gdnappaoi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/gsebzoyfd.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gewiegzhk.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gjqtwriju.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/ggxvixhvc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gkectnucl.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gjwyhjaue.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gitlapfbo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/ggyjumeen.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gdeegxbxm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/ghdxxwyed.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/grlwdalog.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gfrsvlokg.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/ghimysotr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gtwnfywgb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gyrswocgs.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gdkfnrstl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/gvhhecurw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gomxfqbqr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/guvrvlyxq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gpfiykmbb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gyybdwtvd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gjgenviym.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gmwgjgzos.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gjrfxklda.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gfujublor.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gpgetjkzy.sHtML


<!-- 参考信息 -->