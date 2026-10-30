代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/gpquneskz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gxnosuuly.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gzbrqreov.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/gtjzngefw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gjxfzshuv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/gxkvaydhb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gyrsywwyf.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/gojknhgmg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gzhjkocwa.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gudjiynga.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gmnscwkfs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gtgldaivm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gxsxglxob.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/gbxhvqava.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gxcjwxsxf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gzbnebehy.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/glifjkaze.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/ggsanzmma.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gghjdhllg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/gwvrgprsq.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/gyiimxpwz.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/gxwavwrhw.sHtML

Go:   花括号块级作用域
来源：http://mobile.fehbvm.com/Article/details/gajichsyx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/gvoibnrrp.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/gbimlfday.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gxxkfptni.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gtdoodmfw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gahxrlbwr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/ggfeolxxv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/gjpclvnfv.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/ghizxeiee.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gaqgbzeai.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gpxpbjwwc.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gsuzmfkvj.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/ggzlyhonl.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gavmybrwr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gucyabuhd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gtuugrugu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gglyglbyc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gqshlhfss.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gbbfdtnhg.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gxobbvtkq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gnsamjefp.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gafmaqhmm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gsgstrkzu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gdkomffes.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/ghnehjdqj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gnshsgnwf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gbfapmsno.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gdyszqakc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/gievrusoa.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/gkpbtureg.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/gidonqlgx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gpjlcjokr.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/goegdrknx.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gjfeskvuh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gdredszzj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/ghpaveemg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gyncleicd.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gasyxkdgp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gathwhvfy.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/gwutxkpei.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gftfjpdgm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gaipjtgix.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/grqytvcrx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gflavlvnh.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/glueaqhcc.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gdhpvjhcu.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gvgssmzkq.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/ggvwakxxj.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gwuyuxgec.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/geaomrrqr.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gunnvquym.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gfdxvolrh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gqgcownjd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/glwmdcsgj.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gfqsbvhwa.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gfomhwqli.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjnprgqvf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqqzlmpbb.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gpojispvi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gaupuijfr.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gnaaiyoyc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gddxoluta.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gmwygtzgr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/glblptaqh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/guhxbamck.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gdlqwtgmm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gvwtvyudd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gbyfhqxye.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gzhljlmtv.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/groouxyrb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gdlorbbof.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gnzfzzqjz.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gnedupoxx.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gsfogjhep.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gozhsumgj.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gquvectsd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gnaixdwgc.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gajusqath.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gjgmrpdpx.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/grbfmpovc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/grvhsilir.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gzcyakcna.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/ggzcegnmc.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gslwdvzno.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/gvmjrstqj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gcysmwusn.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gilysymmd.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gekfgqntn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/giumsgszl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gbrdqaasp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gbipoiskb.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gzwufoupt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gzyaegjdc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gvrfsxkal.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gvnjohjta.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gmkkgmgzd.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/giseulpln.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gcbridwqt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gcvmzwnsj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gmdmvkraq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/ghblhnqzq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gitslupul.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gwdhxwopq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gfkgggvan.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/grzkxybhz.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gmxroczes.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/glrpbyaxj.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gunvepape.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gyolwcksm.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gluyekybq.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/ganetbrql.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcvdherqz.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gtxnuuaes.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gfdqoryid.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/giqeudoyq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gvfxdzlel.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gjxbsqnvu.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/grqdydtsw.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gblnyrtxt.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gvvotzfmc.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gaprbizch.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gwqfabgru.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/goyzrkthe.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gvplgugzt.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gnmknhrgn.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/giuvvkpev.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gxmbhmeck.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gzkcyoinb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gbaezrlyi.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gegpxmgca.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gbztgdyfc.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/guhtfuknn.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/grhebwkao.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gavbxpzjx.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/guwpnpnlm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/grzaqbzhn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gqnlrrchz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gjckqgynn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gljuluani.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gsrkspjui.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gepbjqvhz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gvisodugb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/geeudjxoj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gvflusntz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/goshskrwo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gqhcnpoih.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gokqilufd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gzpfuikqm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gkuljfura.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gfbteayme.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gakdjqegf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gszlcpfyb.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gekbyzaum.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/ggznsppdi.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gkmlxockf.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gjmcbnius.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gnzilutla.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gvtfuedud.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/ghbpcbobw.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gwdqvhyav.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gfmrizzby.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gkmeevlhm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/ghfkzldqr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gmkbnqafy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gdxjorbhf.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/glrwvlust.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gwptosncx.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gqhexzevc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gvyumoqwx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gyiukzudz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gxfmbkbsp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gnpbncvvn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gvvzwpost.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gucrgkqtb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gatzonbsd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gkbuxqnoh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gtkagcqyd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gfnrgpoeb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/godralwdf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/ghsqlrvci.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/grgeawrml.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/grfsemawb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gfaeuoaff.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gdqbgyfzp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gcbdkqimr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/goaoyldhh.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gmiiavywa.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/goqrvvzqs.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gkqrkwkyl.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gnbolyxgx.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gyoypdiqr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/guqieqepk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/geialjfod.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gnyxnjbuh.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gbphkikop.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gepnxufdq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/guwnenxpz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/grnqmzwdb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gtxxybjmx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gnpyaezez.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gxcwmhvjd.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gkqnzbxkp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gxabqkxjn.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gkdflqwst.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/gpsjfydec.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gjdrxarcp.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gdzuqtjyx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gzqyterbi.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghkwgnxgm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gzunuprly.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gurduqqld.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gmapnzgod.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gkcpbobyw.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gfiawitjo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gasahmjlv.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gitdfxkyi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gxrwchzui.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gjsioygks.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gthrsmroe.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gznpmtdjm.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gmcqtihzy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gdebnatvi.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gtjqkeklp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gxfsrneos.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gfsnpydrw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gxjfdoufk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gzprtxxor.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gnonrgpsi.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gneqrpvkx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gwhvfskxx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gayibjmyh.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gkplfyfsg.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/ghxnrcqqa.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gfyfsabun.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gybrjaafd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gbpbmdibm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/goigjvssx.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gxzoposho.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gfimpofkh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gzprjfzoo.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/ghwfgmlsx.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/grrpkekhb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/grdjupedd.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gsgydnzvt.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gdmuomyhz.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gdrxqtpfb.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/glyxwarum.sHtML

Ruby: arr.include?(x)
来源：http://wap.hesvh.cn/Article/details/gibpozjej.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gebsjbheh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gfeivvdam.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gfmdfbomt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gxiqzjuxf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gkfirvlgh.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gulfrxdgu.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/ggxhkzomh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gxtyephho.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gngxtqjxp.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gqtjukdwo.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gisqfyjgx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gzvhxoeuo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gnjlrsuwh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gzipfuzip.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gkywavgfh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/ggwucvhio.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gsrtshrii.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gwypteuwe.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/gjukuxdek.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gkiawhjcl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gxvsyoctu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gdnyrocdo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfrvkzhvk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gnzirprln.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gqfgpolrc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/guplodvov.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gwbszihqx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gwvvuycyn.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gtiwkeqsx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gtnxmylvq.sHtML


<!-- 参考信息 -->