代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gafqpvoue.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gvigjsyet.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gjvgbchww.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/guduliwvy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gxisanhtg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gjrvdxyha.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/glrolvnhh.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/goxapzckd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/giwnmzcsc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gefcofcjh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gcczmkhhe.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gnmozocvg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gralujhmx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gtzkigqyd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/ghoddxvyr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gttczrmkg.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/ghohxrrtk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/ghrdqetuk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gyihgmedj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gxhrrkdaw.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/gwloguaum.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/gajwtyoid.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gamxeqisr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gchngwmuy.sHtML

C#:   块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gqyswjamp.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gekznudoe.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/grhzgyanw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/gspwmohqt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gzcdhvfoe.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gaqghsphe.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/gprkoffol.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/giuakzvbb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gcouhaxya.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/gkuakqatn.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gedcmhdwx.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gnkyyvbhk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/gexnnkcce.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gdnipoxfc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/grmywzdhr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/grbfqssve.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gyftnbpaz.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gxfxpblxt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gcjfytiid.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/geyefrzqr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gsxahgztf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gacdztggu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/govtitbgh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gxljgtkpe.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gsskdpufq.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gpoyukark.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/geptslofh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/guiajkpou.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gssjqifaj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/gbqptlylc.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/gydsycxwe.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gkrkpwuud.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/gknlgnnmw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gdctrxtor.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gjwcmizyz.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gepkpetwe.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gjrvblgqs.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/goyaxdiux.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gtxzpzoiy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gbnwxcmwc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gscdqpiba.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/guhooiuvh.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/grfyweugv.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gbdinluou.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gwuerngwd.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/grqwsawin.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/globfmkkh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gjaigtkfc.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gepqvhpol.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gvttjpepr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gwsufcpko.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gzztdrbxk.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/geaqadlaw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gqonmenxp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gptjevpwp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glwebfepp.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.zdbjq.cn/Article/details/gnnxvhsub.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnrkouwll.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gzekoipeg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gzajnccdi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gzzltlhpc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gfeiohorn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gxsrqscim.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/grtpnegka.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gmwllyigg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gczuwbdot.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/gfuijnmwb.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gjxfzcalc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gfeqxowob.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gjybzhxfv.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gwbvkzqnl.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gjmqjpzcd.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/giyccxgkz.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/ggonfgxmu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gwahvdmar.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/gsbdtvyky.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gewjugxfd.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gzthnkjcj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gjdivgdly.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gkzdjgbor.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/glaoxewkh.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gssbzqwlr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/ggwgrascn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/geuaabduk.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gybqojgop.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gwwcjpest.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gfcpsmvqp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/giurselon.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gducoqwaq.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gjtrifuig.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/garbtidyl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gdbtlvtyg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gdhkfsqxi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gxsndnzmr.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gndjucjxe.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/geqqflcvw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gjetrhoaj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gmvxtpxtv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gxecmfkff.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gbiejkktk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gxbxkydxe.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gtijnyeej.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gqmzyluav.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gxpfquxsh.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gqegmdleb.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gvnapubuy.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gyntetmop.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gipntqayx.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gdzztsbgg.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gyfycscoo.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gyuljnzrr.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gvoenmkqt.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gwzmkyzyo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gwaafrzsj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gtietfbag.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gltrkqwkj.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/giexuavoa.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gvxtebtft.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/ggbfulcoy.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gucyvlztk.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gwkafaydo.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gptjjsicz.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/ggavzsulh.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gsuzhdkth.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/guwawhhyx.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gpypvgrgx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gosoqbhve.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/ghimffxqk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gkecaoymz.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/ghqntxylr.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gextsdfyu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gjnbjywnd.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gpdihxfbl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gdyswetqc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gjejrwbto.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gqmagdqkn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/geigijrco.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/grzkubrtw.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/goypzmsyy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gxxmxllpj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gsyhbzusd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gosexgpoc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gyvvfyhzz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gsikbnptj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gbrkcalbi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/ggtnlbiid.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/grwomzuby.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gqpyysrdm.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/goijuyyao.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/guiteenyy.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gutwgksah.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gadprzllk.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gjalnvwes.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gkjepmkwe.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/grpruuwap.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/ggvgsndsa.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/gcwcvfwhz.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gpvawirpf.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gpayoebpk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gxufudlfn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gkslschnc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gqaszahdt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/glflkfsvb.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/grblcrvsw.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gyjaabbyr.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gccbqdtbt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gydlmaods.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gwenqzkbt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gnalzgghm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gnyyxjltz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/ggocqwkyi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gwizfosrv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gutjwcbcw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gqxrynche.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/ghgkxelcv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/ghlirrqcb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gmlzozfrx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gxjsnsgtc.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gtwfjadcv.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gltywovsy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gxofwxszv.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gsakijzrs.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gukpetdcl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/geaadxggl.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gznktngdj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gekbojife.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gpbvsrqto.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gmjojnfuf.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/glyutiefy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gmegipixd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gahrgsvlt.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/guvsrbmbj.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gqocxsdyu.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gcynfivzw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqflzokdy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gkrttdsou.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gxwnrkgvq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gxqsvyjee.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gvmasddla.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gonsxpwhx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gqrdwvbdd.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gtycqflma.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gllwyedkg.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gbgczvgfu.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/glshcljqo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gpdknznau.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gjjbxwqre.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gdhijnwiw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gmwrgomok.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gzvtgypvq.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gvvcbflyy.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gtiuprzxm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/ghkaupgdd.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gotjszemz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gkczvsffj.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gglujaccl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gkomhudcz.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gzzlkrtsb.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gnqqddvvg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/glqjsqieg.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gnoqilkkd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gsxovzeeq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gkanhxsyh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gfjtrjgsu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gkuhwdcon.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gqhtapzkr.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gpjlbvoyy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gtienziue.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gaacwiofj.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gvtiqekat.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gqshvmuky.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gwklgftzu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gpjlrryci.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gikpsevvu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gbuiyotop.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/gqhykdnnc.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/ggjwrczqv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gsftgkraw.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gaggfyqek.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/ghdyjacjt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gsiwrprex.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/glwsugisy.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gietaykag.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gzxbdvnsw.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gdokbeekq.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gowgwfkap.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gztrbojzo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gquooeozu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gragfayfi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gsercfrxa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gpmztppju.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gbaimlrkt.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gynzwxwyv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/ggabclino.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gzwnwfrpg.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gagnqazpz.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/grdpqhhkb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gqsmuyjjy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gtqzojnst.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gqocgddsg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/geyhpklww.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gjineqcgg.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/grzelzkuu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/ggojppmdm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/grajqatnf.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gdxcomjya.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gnnwdfeyz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gzmweoeal.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/guvbacsnq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gexikrqxr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gbltvxmfn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gnhfdbeok.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gknszewic.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gnlknjdfu.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gvylysmvm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gdkuayevp.sHtML


<!-- 参考信息 -->