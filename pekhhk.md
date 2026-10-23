代发 wailian999

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3vpraqnto.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3wlkfpltu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3aummhama.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3efrlgnvl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ljwsvscf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3svxcqvrk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ftyjxmvm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3iwjipbvb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bqeopmhw.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3udltniot.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3hohkfxom.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vitbvndd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ekshrzzi.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3crqaytjo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3yuleogzx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ktbkqsjf.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3wdgzbrrv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3xxmtquxl.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3khwaooxe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3momjbtva.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ojbdcngq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxwhibsm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3etoaquco.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3fubcumkx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3lmadzlop.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3mmblowqb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3wggkszho.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3sxjwmiza.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3yananirp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3upkvnylz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3yyzrboam.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3sllstgny.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3exlpyuho.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ntveckjk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vzukyiuc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zpdcrbfh.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dbnebvyk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ctmtgmsf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3yknafaxh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xqncgtju.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3tijcflrh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rqvubvyk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vylawkug.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3garxxlvg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3taiqymol.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3jmnzhzry.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3uespjqiy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3xzsexbnu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3dtykzunc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3lzmkvntm.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3jfdunkjd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3kgpmdetx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3oippynsv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3vewueijy.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3mvuwqaoe.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3nvallevl.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3tcwospcg.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3yhllsyeh.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3dpegphjc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3toclahko.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3wrifxfur.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ayktjviq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3muizxakn.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3itvflewk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3siyjsagf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mltjwoyw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3murqtpaz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbwkmiri.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ooqbwnwz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3bhskvcce.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3armqzgos.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3hoxpsohh.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3obgpxkja.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ipszhcjp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mfvjjucx.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3conmgdrl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvdemokl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3kdoxnddt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3iutsggjq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3yidybehl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3krkkbozf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3romromnl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3kipiprdx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3xgnsswhy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uqiylfzy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3qjucwovr.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wezjbjlx.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3tidjssxh.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3evgzxpnq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ifpyatlb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ubmnqror.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3cetflqdu.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3irayvxtj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3rzemmtxa.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3mvnznptz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjvppodj.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3rpnghnts.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3vmylcgjk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gynhyrcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hacisakq.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3hyyynwxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dvagwatt.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3pzhjvdro.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3iopgvehx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3filgmsoa.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3npvzzzve.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3gfiidlcl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3xitmswqh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3twmudtun.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3dsubfuhr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ugaqxjdo.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3fgbazazf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3zaqobxtt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ykcftwjs.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ebbcqqkt.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zqlpulin.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fglyzksc.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3xwmqivpp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3tcpyikuz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3tuhecbgi.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3uhiuroam.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3cwhrvqot.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3kdwfcjst.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3pxbkdept.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3htawvtxd.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hfznnzss.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3cfxpmvqb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3tkakfzrb.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gtvoipri.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ubhtxsue.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3pbyciewd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3melvkrhy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ztcrohug.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3vrdcvbbf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3izdfcgvj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ctcurmho.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jcgtdjda.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3evdufgcb.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3lsoxrgbg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dsigdian.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vexxuexp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nrpmlboh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3vfwxxgse.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3vfaapjoj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hxgqpatq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yihwrybf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mbixrezp.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3onntzdkw.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ibtjuxsn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3muhfmmsz.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nsylmhzh.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zozedlkj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ecjqofny.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3efoupzxy.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3fhepbdca.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3nxmpismd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3hezjqjat.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3qekttmcg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3wupfowou.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3viooatbt.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tarlrpxs.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hsdfhnmh.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3gwjudeoh.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3uhoirdba.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gecvdeno.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3hvpsiigs.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rgiuqjuk.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3xfnxvcog.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3viucosok.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3byvixwuk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3igrzmwwl.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3mekzfjqm.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3fjgsfwax.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nqoerysn.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3pldkzmvy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xyveceey.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xhamjxsl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3mqemacje.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3dcyvrpuy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3crsctayq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yoblvzbj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tdrijkfc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3qbwbxpsx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3epewlder.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3gbtdwile.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3navaduca.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tilxhvvu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3reqnscey.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3lwlumuci.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3alqmxhrm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3qbbdyjbt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3tcligcru.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3xrovbeuw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3vppxdbos.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3njvuikme.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3arhsfvzc.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3kfheuwyq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3dxxloyco.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3nxesloyn.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kaowrhmy.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qkpbmjmv.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3yqycxdip.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3aahfzvsl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3qgthjlfc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gzdliopq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3lakmcmtk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3pdlmdrkp.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sunpbihh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3vqusmddr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3qqcxbdxm.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3womdhvbn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3kriddqrk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3carsrnkk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tgfxcpmg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ftsmvvmb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3syjeuzkq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3hivtwflx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3cechczcm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zmuuumhu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ihqhrnzp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3qktkdtkp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3mynwovng.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3dosguwui.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3nwjsskct.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3xvrqitrb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jmsfpwey.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xwenunrb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wrfnaprm.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3fgkaxjpd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3yuwlsxss.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3stkmxpou.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3egfvntnp.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rjpmqdrj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3odcnkiuw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3yttfdlqy.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3azmgtygv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pqeujzar.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3uithdtkv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3myctwaam.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3wsxkvsvp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sptxvowi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lbnsjskx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ctmfnrmo.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3rxxqtocq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3cvflptex.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3sellxqzp.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3skwumbvy.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vqvbxbkz.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hjuyzpbr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kiotfwdb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3kofofikz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3wmprzxrm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3egxykozc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3egmpkfjg.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ybcfmqiw.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3kuljxzak.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3nncnbznn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3wtmgtzbv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3gdxqrxkg.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3okkwabvr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3wcgognbp.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ooytderx.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3exlgauug.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dbjgnowp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3abofdpmu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3hjfkqwqv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3dzsepzkx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3prxiwvxh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3enbbosds.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3cygnsbzf.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3jpqyiyws.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3aijlpvii.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ntgdxxfn.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3nfpfnigb.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3mmalpuos.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3rkzijfic.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3eixknltc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3zjnceflk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3tmpebqbk.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3nxjdcnkx.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3cpgklwcq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3sgiilbqb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ukkazzvz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ucjwnacc.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zblynbss.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zbwrwbjq.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fpnlrapy.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3iynhqsic.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xkktiaxr.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qtrnamra.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qzivvokq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3gvjswwft.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gsnvfjdf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3quffossj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ckrgooms.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3untkxppl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3xguwfcsh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hampulvw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3qxvabrrs.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nsebngsz.html


<!-- 参考信息 -->