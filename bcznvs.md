代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2szciptcj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2yqholnze.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2veqgcbbu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2uxrkagjt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wmnxhehp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2fdqeffzu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ulagvpfy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2gkpxmkvp.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2osnedoft.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2nuxzoqlj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2hftdwugo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2hxgeputk.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ezdpzydi.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cljbjpsi.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nryijdfz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2gwjvrsgn.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pqnxhlhx.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ggzuxeub.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2acuwbqse.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2grgzwuei.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2evyahrur.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2kjqpcsjf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2drfbfnqe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2nxkmxtyx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2iwgueqdo.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2qefvenqq.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2anlzbtiq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2puohdfmw.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2cjartnfu.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2exmihkeg.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2labkrgbn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2uqiezcec.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2stsruyvj.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2tvyqhzaq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2freauxmf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2wvkqsbwx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rphkmgrx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmqehjbt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2yendqorr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hfdwtlmf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mhhsrxnv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2sfpkdyiu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2lpnzvblx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2hkiwfibo.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ahxrfbxt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2iqfqwsfp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rjaxcczs.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ebfqroik.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2cdrfhunk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2wasaaimv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2drjtpwma.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nmukkqdf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ouiulmth.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2vjndeirc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2rywdypve.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jaqypjss.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2phravnsq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2fpsqwsxm.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bfdrifqg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bqwxzvzp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2wtfnxeah.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2fdxlypkj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2tyxyuskl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2dsnssqvq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2sjnrsstn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2rettzkeg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2lcjrnvsy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ambplbhh.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2uclqkmic.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2iweyiwqi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2nlsqaded.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wejdnavn.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2zjltrgpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hqmrkeoz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2kpoccnsb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ssrvqvkl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2bqjkjibf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2srtvqhjt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2grpckdos.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2fnbptskt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ecsibfaa.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2hbuqxaon.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2alccmusu.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2dtsyofcp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2nzvuaawp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2pxthxfsu.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wyhtorgq.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2avbqqdwl.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2lhuwszep.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2guhcxaag.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2sedbcluy.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2evuqtgrs.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2zyyhncev.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jhyymzpm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2nfacloma.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2pmchdmxs.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hwdlrefa.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mphnkxck.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2hmlfhajk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2tyiycrin.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yrwglsox.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2iejjohnw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2epovqusr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tianptkx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2swwtzxgr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2mksqzngi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2pdufjcyt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2sarqgdoo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ymovdnwp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2xawdrcos.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2xqmdahjt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mhhcfrbb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ulugyjqf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2envsveyb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2znvgtwbi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2wcjdyapa.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bllxpkvz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mcgpitkz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tzbqtgfu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ggjmgspn.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jnczviwp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uidchedx.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zecyxgax.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2buxsicah.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2vwnrsysx.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2iqlkqmou.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mklefrhi.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2awauzvjm.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2jxisdgrb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2tmahxtoe.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2lxqzbzyn.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ghjhbwll.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2krraxfzy.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rrlicrtx.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2maxxvwmo.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2bmuuxtyp.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2phjrszsp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2wsutlwff.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2bigcpyir.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2vqjqwneq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2hwsdoemb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ffinixgn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fjdfylye.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2yhxasfkk.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2snnamzfo.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2imzxqtrh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ajjmicko.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qftpabql.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tsxtuuos.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2kwfrjfwh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2cshwigli.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2xzqolqlu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2irezqrrl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2pjukhkmc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2dmakxubc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2iwynhvic.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wxtqukpd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wbkjmdtw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2gkfjaneu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2gpcxhlzf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2jntzdidd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2qchgvljc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2flwmyptv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2jktmover.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2xnlmgplr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2kocobdka.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sejlhwok.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2bndvcizu.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2joisohwk.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ockjoupt.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2dyvzkzvw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hcbigqlq.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wkztvkuo.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ynfjgaxx.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dhyrlcuw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rgcijity.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ovfqxuvj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rpdvzovx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2azllvnne.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qnckjswb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ldscnssl.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ljvcfmnu.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2cucigwgn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2pyfmrvzn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2myzjodsm.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sqwanzty.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2vtgywwyq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2mmnahmir.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2zqjmdxis.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2wmmhfgwy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kdkzlyvm.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2jbkjluoi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jjaawxex.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rcycijny.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dtbrykiz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vgkwbjsj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2liykbkgh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ftforaxf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ihrslrqv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uftbbqbu.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2zaueywkx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2odxharfl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tfxbmksy.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dsxoskfo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2yssinspn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2emfrylpd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2netdgowb.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2jnmclbuz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2bfmvtboa.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2qfqyuzfo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nlhcdqyg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qojgoari.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hxavfrob.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2owqsjrix.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2hycxgimu.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2uadmuyil.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2akxzkcul.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2gsuinagi.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2tfvablbh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2gquwqlnu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2iycarrsw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2nemjrqds.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2moaapyrc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2qiexnnkc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mvmefebb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2aawgfeng.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2xvfhbhbs.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2gskcgdkl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2jdxicjoe.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2xdoygiby.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2eduecegc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2zbenqegq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vljzgwbh.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2fszkzysx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2iwypftng.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nunudosk.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2yftdshkz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2pquvausq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2dmjxfzaa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2vswzbcum.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2dokgfwzm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2pbtmfnws.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2mikytnoz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2jrqiqpmy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2glanurpu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2urlbwwsc.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2owxdwcrk.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qhlnyhuo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2nhmgwfdu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2bsfwdsxu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2vvjhbpad.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2mskjfjwo.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2jmsxfnjb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ehuiqtjq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2prviziqg.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2coejvvgx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2wcxxecak.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ldnhgqsv.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fvilssiu.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pargvhdb.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pyxbqfoy.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ahntmrid.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vpnfkhlj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2asekbvqf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2jzqedfvp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ohuksytn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ivmvqqlx.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2nbqziwaj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vqbhqpca.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2upkyyenq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2bmosdvrh.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fwlrbzto.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2kxppndwl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2rkfwikgb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2piatidiz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vrpbiyue.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vcyzbxmc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2sxzfhwkj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2lntrdnsd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2wigmqrfj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2rfmkjprh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2rdxpaqwv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2irorbhmm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ckoeagmn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2zjjaimhs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qrjbxvha.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cgwkyyxq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ygpobthy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gahzurcy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2wlsxvbgb.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2gcmhknpz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2mpwqlkmq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2szqfzqaw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mmlkxqnh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2jkxkostn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rlogsedf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2zjsznpxk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2axotlfmg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2pelsfcvt.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2uhhrggtq.html


<!-- 参考信息 -->