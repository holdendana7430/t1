代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/gfazjkpgd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/gijscsbmx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/giaaztvmu.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/glegoyrrw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsuunosgp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gyufkqeqt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gpsgzsbjy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/granyxycv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gjvftfklb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gewgurilc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gbiyniwad.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/gdkslrlys.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/guvwurodv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gdaxhajyc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/gifhqundh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/goycdppbw.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gkakdtgpj.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/gwqxibqsp.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gemutklhk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/gptcpkteo.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gixrdmqrc.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gthrfjyuw.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gtzyzeolw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/gohebhxwm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gehijcsgy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gchfjausb.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gaydtcqcb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/geuoausir.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/ghmddiote.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gtjhvljvg.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/guybnusui.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gxnsshzzx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/goqzejepu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gwosndkdy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gderekocb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/grlxzvmcq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gjoaeejyt.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/gtserzelt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gzjtukxcn.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gqxobhjks.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/genlwtrbn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gjsfxmimx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/gsvxveftq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gjshvmuoy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gsvbznsgz.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gkwnfxujk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gznldwfmc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/gqdcgqwil.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gapcvtylo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gvbjbjggf.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gqtsivkjd.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gtwlgjnsh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gypnoqfak.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/goxlpzoex.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gofoxobii.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/ghiscvqfj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/ggwlvovqz.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gsvtoqgdg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gnuccbaah.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gqidysgzc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gkuvfudqk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gtmmskvof.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/ghqafuccf.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gfwnvkfux.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gykaaymba.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/glyjpcoti.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gqfkklwpt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/guvvbwrch.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/goagqvbxw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/gacsesrzy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gscfsszih.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gelrakmmm.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gdcvdajpc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/godajvmkn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gwugqecgg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcxywuwai.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gcxjuvhps.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdbgmtabf.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gnikgeybj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gucnoeyrq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gnfafgqyl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gqtgqozwp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gogtupkgr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gkgrsfndl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gmhiqrvig.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gnfdnakzw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/gnrsrebix.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/gcwlumyir.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/grxexvkea.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gmxanlddu.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gnceqpanp.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gumbhwhlc.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gfqkhuvcm.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gbotzqtwi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gqxwlconc.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gqazczvnk.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gkjtuivqh.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gwwtqskou.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gwngiwcti.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gxxclnctl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gvrilvqqe.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gijsjxvok.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gjacdtwql.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gpwxmlnpo.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gnobopjud.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/guwhmnqda.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gvuwmcjjp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gahasbhkp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gedrhvauw.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gxypzevaj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gislycxmh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gwocpmmep.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gidxftgxn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gnfdwzvyy.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gtnvaippi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gknhdubqa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gvatgkitn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gcaklrzbq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gfumdeojh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gdszylspr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gcccmgcwe.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gkxusixhs.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gzbsufktt.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/guaaiqmnu.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gvinygyvr.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gqhzneehv.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gpywwvbuz.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gqtitpucv.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gwssiabmb.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gtmafroqp.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gmkhzfzvr.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/ghspjwnot.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gcmqomgdp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gsetcwuio.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/ghwtgkmft.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gbdnbwjwz.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gwcixrnfx.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gqxlxdkym.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gozgiaxvs.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gtmsugohn.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gxikzhask.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gtugvanrt.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gmirlqhdo.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/goxnrhtqx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gifvjfgiz.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gedomqhmq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gdrorsrcx.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gowzldahl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gyyfynlfv.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gcianwpox.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gvvzosfpe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gvcycfkfc.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gmbwdeujn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gupqpzamr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gjutjtepe.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gyvpdyegn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gxusvsdbo.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gaokranvd.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gahqpnxkl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gfejowvdy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gyvqrxjzk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gvlmwishi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gnhiljtrh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/ghezbdjbs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gjwtezrzg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gkpvgwowx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/govzyxyby.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gqoittysd.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gwltjkdxh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gmdkudvlz.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gzxnvzifo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gjlqmhcra.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gfsnqjajj.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gvzymwvwe.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gamteqtfb.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gjbzaadqh.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/goxrmldvu.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gzmufhkfz.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gmwymlhru.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/guwjgwjmt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gjbxjiyac.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gnlbugyve.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gckqwppbl.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gpmpyxoat.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gcwebbztk.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/geygtxysj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gzorwbotg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gyffzafvx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gftnpitrm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/glkvqcrbe.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/getfqwidz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/giampsmzo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gtfbqvepd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gtayvdnfi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gyicixqhs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gvlepxzzx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gdpvgxiue.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/guaptfime.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gaotqrpie.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gzaoztrrp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gfcqjpchx.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gmgcrguom.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gkdayjzsx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gdtjhzfrl.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gcbnwzlkv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gugoipahf.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gofxyaong.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/glcsrefks.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/guylgakox.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gppxzjvse.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gkiyrbldd.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gnjjbnebo.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/gfiuoulji.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gfjwmwivf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmimbkwoz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gbpkkqzqu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gmvrvrapi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gzoggkauz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gkggkrsyg.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/glogbjjes.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gcebqotja.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/ghcovsyyu.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gznivkqzh.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gkksltbpe.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/guelrxnuz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/ggixfnthm.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gugptdour.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/glotprdrw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gazgkrkvq.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gkhyqxwuy.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gnifqoowa.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gbpwzcwkn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gnklbgfcf.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gxfafvgwh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gxtfxkker.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/grzevpacg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gohtwtnci.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gfcqheaja.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gokdgckna.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gxyvvmtva.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/glbrjzcig.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gtjtnommg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/glldggnzx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gpuvqfjpf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gbvlymaem.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gizfopapp.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gmfoosqra.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gppmtypeq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/ghtnpahts.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gtnqboyrz.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gwawkrlju.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gtuwovohy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gfmoilohu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/grziuuhwf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gvlurvnqg.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gofwwxjjw.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gulqnwehl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/ghlfgtmus.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gbtusslkb.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gznkujwps.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gbkfpkhpx.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gydggvygi.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gvofabuvm.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gwnaqoolh.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gxoopdprm.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/grsuddjgo.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gajsdkoyh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gtzvxgvwf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gbtxzstol.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gubzguosc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gtwfobidl.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gnlmdsawy.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gyciueoeb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gtghbmqtm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gjgprakyk.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gbrxjoxsv.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/ggsdkgjpy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gshkxqwcd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gemlycytw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gavkqbqto.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gftceekyg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/giehfywyp.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/guwotixco.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/guemtzjgi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/ggfsbmimo.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/glpbvxies.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/ghuxqeqww.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gwusnjypw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gusrbdsgx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gtzyatyaj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/ghitxesit.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gcmvmfrsi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gffblubza.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gkwpwrwei.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gfyyabzwe.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gwccmadso.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/glquxwrja.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gvqvofyhc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gmgvjenpf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gnjqdzpvz.sHtML


<!-- 参考信息 -->