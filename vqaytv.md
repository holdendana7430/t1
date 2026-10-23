代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lrtzwnaq.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3aqhrexxx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3cyjbfjos.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pkokehde.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ycsbirik.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3qxptgdux.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sedczoyy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3bkabejll.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3yqcmdnoi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ikuoxpps.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3mppxupwn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3vzumhlsb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3oxzgnafr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzhdzijr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gzsbauwf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3xilabtlz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3kevexizo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3oghamfae.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyqfbrmx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3cuwttiso.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hotjajqu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3hepkqgef.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3hndbzblh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3czagivcd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3uwjjaftr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3lawhdabv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3boyzcgtf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3idnltqje.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3kkjzufve.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3gfkygscg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3mgzbmste.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qwetvbbt.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3nvuxrujt.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qhfhwocy.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qopkpnpm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3tdlzxivk.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3khejzgah.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3kidkbvyn.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3rkckosxy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3pmcqmuxy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3kztvvins.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3kuxvscjj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3yncxqkaq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3gdjrviik.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3aywpheeg.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3cuderoyd.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3sftlhrzf.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3denjwyhe.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3wfyjwsnx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hlrjpdvq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3vxzhbbjh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3bpqvmusk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3uouxrgik.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3utahxecn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3aefhnpsj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ssdigyfq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3dhawckcb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayfbiigk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3dkwfhnzn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhmgogja.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3raasssnd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3wypllsmz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3kyxqsahu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3arkcfsml.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3sicsiigi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3lbxvobno.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ouopzzcl.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fcjqvcsv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3stkjldae.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3njcjehdz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3qccljqop.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bbyyaedk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3zzlqakjc.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3zvrnplkg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3uwdbonjq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3rrfeuhvy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xynmowxo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3utzrcmfc.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kjjnxmaf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qufcesuf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3umgermkr.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hykylosz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3pvlilvyf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ugijuvad.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3sqmrmgwa.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3nomjigob.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3vxqeswxu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3jcovgurz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3qwsnufbo.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3kfquirfm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wknhuqcp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lgjddifi.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3wwtwxbce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfwpgzaq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qzftqkhg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3drkenwol.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qblrydbp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3rfnbxlcy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3qbhvassy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3oshlowgk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3umtopiim.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3unpfudle.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3yxtpgspa.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3iyovmzum.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3rtlthnta.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3pwcuzvbu.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lnmtolme.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3gbdyhinc.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ukevanmk.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ubfyshmv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3jusfkyob.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3qqevzhpm.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3rgvnztuy.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3drbovlnq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3fwbeeujx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3nemvgucc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jneoysdz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3brfcvnqw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3nbuovizi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3goqbnhqw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hgmhjvqv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3gbpmsunn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3srixjkqu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zzuwswcu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3fokqddhl.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zkrhcjgb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iwkehnti.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3lstgltaq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3wkzjwgoa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3yjgpoqbs.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3fqkpdqik.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gvhvgtbs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rrpyvvpv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qbqziwbe.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3voapcatk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3zdabjqny.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dzcpubxt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fscabdlt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hvujppks.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ubylycsi.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kmpyzwxd.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nwuqighr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kmqmlypw.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nrzkkxsx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3bxpvekhr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jrodyryx.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ypfxjbwd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3cvllbrnp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ipfsiclq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3xgykmaym.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3yzzqjzkg.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3chawvhix.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wclalrhf.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zxhcbnzc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3xzvcyekr.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ifcdzhis.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3kjkkfxrg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3msofqdti.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3miklxoml.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3xvcpxaek.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3uowxghlr.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3kqufgapx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3pvbcenma.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3rnyywefc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3learlepv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3aiolosir.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3qefgieui.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3osbmbbpv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3cavjgkek.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3jpyeoykr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3kwnfaryu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3tsfpsmsi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mjkmdott.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zkmduxhu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3oqkoilku.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3iiuuwlrb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nkxlckvk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ebinqcwv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3hcstcxkq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3svvnabvt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ldpzwolt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3bhigkrav.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ejveooty.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3fosaazip.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3fsqwrkvi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ftwovruj.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3shpktrsu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3deegsxls.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3jhqfiuwr.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ttsyrgdi.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hdujlzlz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3mdeopatj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ynvnwmjg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ekgatbhj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ghkckvjz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3njffzbur.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3sddwjdqj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tsisakkf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ycyapmkv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3prjlxmaa.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ijbalsay.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3gkmoiuhx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3shufplha.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3riahvaxv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3jxrbqwyg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jwhljknd.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aqnnzxoy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vzsmsucb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3vlwqnxgf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3evnhedva.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xddwizzz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3tmlrmeje.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3swagstkm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3audefspf.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3cxpezprv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tdrqqxxo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cmztqmfe.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3bzrpndvx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3coslmvzm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kzcqbzgu.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qkwflqaw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vwueuunn.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3tgxaqemq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3tdiiidwv.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3torjeuja.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3iamjxemy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3zhkczcpa.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3bihfmnvp.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3xmwvcbcr.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3rlhlufbu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3aiuzeros.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bskstuzu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3oinyqing.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3erzahdno.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3idrymarj.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3alsqlwdo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lyeihoqz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3yrmhiunl.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3inqceteh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3rmopawed.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3sxczfbrf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3xzappxxb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bdwcxgvr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wlcehvth.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3puuupibj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3dttrtpvn.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ezwyzcgz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3zgpbhgsg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3rchntxdx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3lhshrfnl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3sdakpfsk.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ebsqvnqj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vxxlegbu.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zpwdlfwh.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3nlponefo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jfjmqhoe.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3htagvlrx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zltaxgol.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3xyrxirei.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3iiidknyl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kjgatnwt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3tkqwxiic.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3bfahidsv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3fbnefmyu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3refngtas.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rsgsesrv.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ykbbplrv.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ydqbiyeb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rirnfxia.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3wtidshpi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3sbjnjini.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3rrxszcdy.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3vzsnooav.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3iyausfeq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3xboatxbb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jrqszwxo.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jcwqnrmg.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kpgffjlh.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3omgjswke.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tneovkbi.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3coltuigp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fppvvwco.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hucrcmqe.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3bzaqdrud.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qvcpceff.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3szbheyhk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3fqyudicp.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3frcxcvak.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3zjdcdfdc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3psfqgkea.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3mmhoexwv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yirrxksx.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3qjcymawo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ogilhgkq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vlzwzrub.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3whqbmtcs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3twkashvj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3bneqyfqw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3yzbyoyhf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3xzncwxuy.html


<!-- 参考信息 -->