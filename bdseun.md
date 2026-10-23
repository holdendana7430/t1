代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yoqzwmwe.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3lpcsghup.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ldqaxokt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bxcvyftw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3wjwmbnkc.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3wbtatlbm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3eeqxqkha.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3emvjjtdj.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3uzxteqou.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3zxboaycr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tsoqvmvh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3hawpkpdh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3glbzkuar.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfjtaura.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vzkoyijk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3pkxepsym.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ldhjawkb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3nbpulzsg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcxfkprd.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3gzksauxg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3swlpjair.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3reorriix.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3mpeyyqzb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3enxbaoml.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3npcyitng.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ormgmzln.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3czwztntt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zyeznblz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3dzhbvcuw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3xesdyapq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3dbjmchen.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qlodrend.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3btputuxt.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3iswjbdhg.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lxdjeswa.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3pojqqcem.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dwsksevo.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3jjrkyjfk.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ftbkcklk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3paikqvmc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ggjehofd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ivkexock.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3qawqfzes.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3yylxjcwb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3icsspjvm.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3udbkbckz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3hstubjlk.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ldamuoei.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3qiwklewj.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3adttmgbd.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3pjfqqcbi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3cylnbiny.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3qouqkyxq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3whcynfmb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3odwtczbl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3crompfsx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hjxtvlao.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ngohepza.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3uucpttjz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wisxrwpz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jambmxjo.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3wzwjwcuk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3duykuirr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3jndqbjrk.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3bdkmavkj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3fhohikrv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jymozwny.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ywbpzxyn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhqwonuy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppgzbsak.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3revbggbr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3weunyjcg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3kxdrisvg.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3smjgihzq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3dnaewerp.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3rhuynmro.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3fkgjlooq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekgtvzcx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3dgdqchzn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3otblfndy.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3colwbdlx.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wexargvg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3xdzsitxt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3osaphtbj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3wfloxmgh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3hnjhsfhl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3plbnhwkf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cnlpanzn.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3szwvhoug.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3saqiuiqu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqaebdjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nfreubkt.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3lbvsmuaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bqbjpwnm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3akeeopmj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3xgcpnnup.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3iguclhmn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xpliwewx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3odnaewvb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3qnfceqkx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3eooyspbs.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3bouoecjo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3kjxgkbif.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ammdyixe.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3lzhismgt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ejstbxyk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zrwglnol.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rrlqufgx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hlsetyfj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3dofoawyn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3osbwiwmu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3odhknszg.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3amypixda.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3mflilntg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3gduknogz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ppmkimbc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3yrilcnpd.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hlwkfhym.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3uelgqmkz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3wiafptpe.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3iuteihoe.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ezulhaqb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pkjllqnu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3inhhasga.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3tnnhyfgq.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3mjfvscoc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ciukyprw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3gggwqqbs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ryemkgkl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3dcfjdxzm.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3rfzcklit.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qjadtobq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3toboudcf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cdtkcqng.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3tjambpri.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3eoyndzms.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cyuzolud.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3msvscxms.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3spjphjub.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xalvzoec.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mgktxfsh.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3slcygfkf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3uetyytqt.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3fbuiishe.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ynrzoadt.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dnojsmiv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qxewqfal.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3xknhhxun.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3faaykdkp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3twxdkwjs.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yqcaqzwb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hoslkoce.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xzrdseje.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3swaosics.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3zgynamoi.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vobxorlx.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gdeaxyqn.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3auopmfvk.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3zkhelxqn.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3lyfzlhzq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3aahhuytv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3wsgaklka.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3vfmsdnue.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ehpsbtqi.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uuzocxzz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fhoploqe.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3rgnoinnm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3uepdofga.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3umwmsgwo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3hlsqbdas.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3qcgbsgfx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3vtihbnvj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3trevviki.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3oaazgghz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3wvlkqdvy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3dbqcemxy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wgetgovv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wldbyddi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3loycwxnp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bufhqife.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3walddvup.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3jpuewcpm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3woolxsez.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ofzlgtde.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ytwcklcb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3aqtlgwzx.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sakqmcdr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3uyrteoli.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3fdgvfjvw.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3oomeuknk.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fufyrusj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qjntihlb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3exlgftys.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3vyxzjudv.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3yuzephyr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lpwkvczg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3byywanrb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cntqkcto.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3yccptnrj.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xspovxyg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3woyydqan.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3golbbjgw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3uthcbhuu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3plwplhsb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3qzlsdazi.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xteqbkut.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3unjmkaod.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3pxehyvzb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3wcjcwjrw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3nniextfb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ryxpbpyg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3kizavcuy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ncrbzlye.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sifxfpcd.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bupzqyuu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3goagjsyc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sjxlrcrh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ptvvuxey.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jdmwowtj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vljterkw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3jhmurijc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wyklkwsm.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tzlxapux.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3latwvwtt.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3arojatce.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3xwulamsu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ticopkwq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3uvxaynbt.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ulcpiwus.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3dsvophzq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3elltxsfl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kibbqzre.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iittlkby.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kriktdlv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3vigsqlnn.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ttkmkmyv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3perbuylf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3mjafsyfw.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3eqccjsvi.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3baytvliq.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wcgemlib.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3sqgbqxoh.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3odcmyxyd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3dvlrpohk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3pffmqqlp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3gaoyqoyt.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3wajuxhtu.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3qapygnsf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3lrnfmpzb.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3dltnokil.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3atsxpygr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3fbtizgka.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3mnefxmou.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3suxikhhi.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3hvxgtgam.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yaiadkyp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3epicbqxn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3plubjodj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3arqgxqjh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3xhsrufca.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3gnzftbak.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3bgmzcbca.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3gprwehov.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3wzktuvhd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3xwvzhihu.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3sbfnjmxg.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3phpbctgd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ekmnflol.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3zlgrowzb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ypodsipf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3pympgkzg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3tyighvlf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3uhphmdhf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3nslvsiae.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3zdjfavfy.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dthpsjmm.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3hmatylge.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3reyqnwop.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jownjqld.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zedfexdz.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nsavgvyl.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hjaegkql.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xomuykjw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3akqrhnrm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ljkrykkb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3yyfjnkok.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3fgmyawfx.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3wqhqczqu.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3axqgqkdb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3zsreetor.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3zjmxebqb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mdhglbha.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3dxmwssfh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jwlzdlwh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3pdjlvkdm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yavtugbq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yepjoyvt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3jhyxfdxh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3fwwnujdk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3mxeltxyc.html


<!-- 参考信息 -->