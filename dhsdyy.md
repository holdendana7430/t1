代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3gebyrseg.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3rxdlpqde.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3vqypnjdt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3xgliutgt.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3whyzbzcx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3yhkbnlsg.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gdajvewi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3nrfdholh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhfyvpuu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3tmnpqbnz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ujyhgmlo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ziqanydv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3xfcdhist.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3eapzhhdw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rakdczlv.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3xrvkbspc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vuauhccv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqaghcmd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ugduoksq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ynxuwipj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3yeckovqc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3rurtbhog.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3erofhekb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pcrmzjbe.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wbvbibpd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3rczmqnoa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3gahyqrii.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3foegwvsf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3kujrxkng.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wgunlgli.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sqoludjl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3surspqqm.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bozdkpls.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3tvqnklbc.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3irauggdq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3qltxmpec.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tfsdidgf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3cvybfafq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3wlxuxpxh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3nxfqpaog.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3mxsrpxsm.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3iarduzsk.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3snjgtqnq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3bvcxbzhm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3kfakfhil.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3lfeacppq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3gtibqlea.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3cmeqamzh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3egeevhsh.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ahfpvkcn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3drhbetla.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3fyavhiuj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3chsmeqqs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrnzpvmt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3tepshpww.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nemlunwo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pnxjfmkh.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3foeokdor.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3opocyjor.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3plmjvywm.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3nimnnsgl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3vqqvwffd.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xfgaqaag.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ppnxveyw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwzqxfcl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zaordjoi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3xbtifvdc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kohdcljk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3bjntnaii.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3qqmwxzts.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3aphusfei.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3lxiqmgru.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3trwettia.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3qkvtcxld.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3dijtjldt.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ncnjxryy.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3nocyfkqq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lueyyxhz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3wqfgsnrd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3azfjtqan.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3plkgvjts.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3eelmolzj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3vyanvzqs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xnjpizhc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3tjoppwst.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3wgxppkzs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3joimonao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nuuvbhmf.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3iqofmupe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xdenlgjy.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3xcdofkyn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ktyvxorp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qfterarx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zjfsnafl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3qptdecfd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3gyuxrtcr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3mwtqidxx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3cjvendmx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3omcpdenq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3mzvryquw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3mfosvgir.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3xzkjoaje.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hqyxpmfj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vjeagljn.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3oqmdwapd.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yaetfuwx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3kdxvoapz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3feiofhnh.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3rntzexhz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zxazzozm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3tjymodsm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3xazisvjb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3msayjbvu.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tpupmtjd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3yiilrfuc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3oywthbyv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3siiijyta.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3watdyjyo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pidytzln.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vtxurcms.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3vfdsycjz.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nadibpes.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tpgfnjrd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3hojximpt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3oosrgmhw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ibvlgflq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3dpgiaqgl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gdemxbdj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3axvpwwod.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lumxqahz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3owfsbvio.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3hrbvkqkp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zkmfiyfo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jpsvlgqu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zbmmkuzs.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3avqebolc.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ctucdeal.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3itzmbgpl.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3uacdzzsx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jwceozkt.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3llrwdvzl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3orouwnzi.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3wugulomc.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3zwsmzvzh.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3oazcvcvo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3arcekqjo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mohmycds.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3yfmolzox.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cjckfppj.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ihxjsijq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3pbdddqig.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qhsldykj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3wdcrbkuj.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3vtvefkdr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3htoiiufv.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ysrxiriz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ivsmmqoh.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3lylnsolp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cnrxbixp.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3lwlpekbq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3uomqdhst.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ltathdek.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3pfdqlrxd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3acvuyjtt.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ttwkvosc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ikxqhtsz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3mhqvducz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3kuzturff.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bhefywko.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pmuaxgsb.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3gsuiwdwy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3vjaigfvd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3fdfkozvl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3taseaxim.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3vyelifdy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3dnwtssks.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3wtmduomc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3tqreigwm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3liocixtb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3reqpjvhz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3rrmfapdk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3icgscxyr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tjdrlzza.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3qmixwjjr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vhixehix.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3bissvvxq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3jiamuzoh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3eouttgec.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3svvrbqvi.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3afwzdazz.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3vjzoahvk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3isgnxmds.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zhtxyulk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rlgdzwco.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3xruewniv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zhetvaku.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3kjouakrm.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3xkmwnjdi.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3uhnihhrz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3apdlurjz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3focjpkgz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3enhdopdx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3zawrktwg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zehebbhy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3jrqrkiln.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3yezygnpe.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fagxndhq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3gyrptmeb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3wbuitgvh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3tafkglak.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rfdktjgu.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rprxfriz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vvrlanza.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xxnhonoc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mlaejrqz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ovqqxmhn.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3azmvrrgz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mdrcdscq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3jmdvqnel.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fszmpgdq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3oiieucts.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ujktpstj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3nfhudvci.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3zetteypk.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rhclouno.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3uacxxbxd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fkanfuzf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pvuuhdhp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vzxhucgd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nhccxgbl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3njcfltcm.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ymrrahzc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ovbfzfzs.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3beobkisp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jixeenwy.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mftdyhiu.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rxgkwxmy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dgivrjog.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3fgrmqedk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3vdtbuvyc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wzydvqac.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3thizpxct.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3bzpvumky.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3iotfdbgr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3kyfqzoyz.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3cocmfvxw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3sotlamcz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3fvqqibuj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jluhslqe.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3yuykyleq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3btmyzwrx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qkqadkxl.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3dcessiia.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aftxxluv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3gwmsprwn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ozklsgzg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3dvqexczm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3czmflktc.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3vkleegaj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3pfxoereh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3wpzeqqzw.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ijlirxcz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ljazwscx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3aouyrtyn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ucihgnjg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qsshgisx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3xyazuryo.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3zhcjyoxb.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3harjegjx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3jlsjiugq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3amyfbitf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3opbbfhya.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3owuwpmjn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bhkoyusn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kwvbtfpg.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kpjceqrq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cvmictty.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vrjvzwof.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3olycsjjm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3evwumkgm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sgnuosya.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3hrbcygip.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3qogozybo.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ncryznkg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3admtrhqt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3uafmgjll.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3llsegzve.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3wvycjerw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3tpmowjmp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3cdtypuyu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3vmpfjkqz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3idudrtgd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3crfzmnbt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3rhfhacof.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3wkkndokm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3nwqgbqfm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3eejuwabc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3thnwprsh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3nlhcrywf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gtlphuwf.html


<!-- 参考信息 -->