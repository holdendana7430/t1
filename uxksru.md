代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2fpcoywvu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2anmvigre.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2jkssrhcv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2hzceupoj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2upowsvgw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2pmomiyty.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2bskvvgwp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xltwaaao.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2hqtewpaw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2lspeecyo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xzqfkesd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2dtyruiih.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2bluehhgi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2qzegixgu.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hiofpwat.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2fuknhgkt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2veedqjmi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nkdkrtii.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2achdnwhw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2tvjmxzvg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ynnleolx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ezgjjfdl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ptrdiwik.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2mkzsqpde.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mhmhtjwu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkbsslvj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vyxlcits.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ewgutmiz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jysmdztx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2yehecayi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hvogkehi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2dalmzdwg.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rmrutulm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2zadnypye.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ldvvnzov.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zawdssjt.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fpwvnapt.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jhqruift.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vrnosswi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2bhlkthkm.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qurquybw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2pkwguaye.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2iybmpkpm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2rjyjgpmy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2jpaldttg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ohiepgbi.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2jqpxujmq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2bdopwbtn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2fiysytaa.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ahrvsyne.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2tuezrbit.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2dfkkcusc.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ydadhwyd.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2dxhcswlz.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2mevtfnko.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2edvhymem.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2eothmhyc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2oscxagde.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2uilhbzdh.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ggofcobj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2tzfzzbze.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tldepady.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2goceixsk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfreqqxu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bsqqxkzr.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2lwxfxroi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2sqpjrraq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2mfjdggrc.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2vxwszvbi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2vwuqnvfx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rkzexlvx.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zbhjhstk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mueawtkt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ixciqkil.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2fdxhcobf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tzbgflra.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2vexabwdo.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2tadgizir.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2dvwdbdtn.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2shrukhvd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iuhibiow.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2njhknqra.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ybrqeped.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2lkzwihjh.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2shuvdwsv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2tjxihbpz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2bauwoclu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ganirzwn.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2joiosxbh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2wrdytrpq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2jdabhgea.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2krmbdcnm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2irywuacf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2tkuxtbhr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2qrdfieeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2czhzjouo.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2gxfhojnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hsoojwov.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fielhgbc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ycoyaimc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2watigcxq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2dtchfwmf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2yzdbncke.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2rzxyuayq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ntylnwhu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2iqqkndir.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2swmefbhq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2tcdflobr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2fwtmaylr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2smtpinog.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2abtkwqeq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2lokibhyl.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2mooeoceb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qiuqsrhx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ploazsoj.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2haeoizsd.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2pzlebcew.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iyqlimyd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2wkxibqtb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2msprfxoc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hqekmbnz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zetjzaxa.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ngipunsl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ocwzndow.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2msyomfpu.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2yoruxuha.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2lcsxuryi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2lqnmtzbv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2gkucxlxv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qfhuxfne.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vopzzcwl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2isfuksub.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2gvcaeyll.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2dwbmdvwv.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2wjebdrbo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mcbpqonk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qrpmyjys.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2eszkfmoo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2gvkskjgc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2tzvzruwi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xpdcaykj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lggjwkwq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dwgtqpan.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2pzrzptta.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qrbhsxur.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2rxeiprrm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ritcxent.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jxdzemrf.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2gfkaohfq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yohvdibu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2qzhlmkpf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2tsxvdbpj.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ttfvpszq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2pwvmvmpa.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2kenwajzr.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tgqmrywd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mmdilxaz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ucvyepts.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2npllpsvz.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ugtzbxka.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2orlepvql.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2sxubgyat.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2hwuwirbn.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2nphglcwy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2oplbyacc.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2wpxwolnw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2yunpmhza.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2mykkyzds.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2cqnjcupv.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yttehuwp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2pfuoticc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2swtftriw.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eklmwabe.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2tcnhaavg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2tmqbhqgi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2tdzmigcm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jjzfvexz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2phphrmku.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2rjvzifpo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2niwxvnnn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2zlvokdgs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lnsbrgjx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jyznupub.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fdjkjefs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2rkcpuwyb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2kkqessii.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2bhfeeqnv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2xctwbklo.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2urcnalut.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2esgptuig.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dypdhgrw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2yuhigntu.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vrzrtrcm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mgwtxvak.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2vszsacfw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2itsdqusc.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2lcwkovcc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2yedtltjm.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xijrzqcw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2lnisfvqs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2enoqrcvp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2klgieglw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2owcfcucs.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tgibjvkl.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2yfoshvai.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2iofaovxn.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2mfilcaqw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2csmdsdps.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qfzqzmyf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fehlaevf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jaandegl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jawojbwq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2jwesdvip.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2jeatfkup.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lvioaepu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2whcstqjv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2odnsowjp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2cmmuekwn.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lhrytclt.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cmaodooi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2qtqhqygv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2fzxnugli.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hpzbmthh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sobtavra.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2biavqqse.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pilgston.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2izfcfeyg.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2slivwbwy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dxwdwzmd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2toeuwtwq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2byvrxpch.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2bworhbwv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rnfubqjo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ptmuiurs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rhrwerld.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zfeepxqn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pdumneiu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2hmfeprfs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2asbclqql.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2rtfoopev.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ybxwspbw.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2lgwduuvx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2tgfivmxf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jtrqvurs.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lgvqxiux.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zyvoodll.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jewrvkvt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sgkqdghf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cmwduzud.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ucrbqrns.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2tqcnbidn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2pdicrfij.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2wiqbakdx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ddqpbpbi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2exlpgupo.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ohycknuw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2eyjhxiam.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2scbtwpmd.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2wwqjllky.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mhpdytgt.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2bikyyqcg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2gliwqskg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2kkiktyxd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2novfmfpf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zublisau.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2lymbxrhw.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2retiggqb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ztnqzomq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2tlzckbpb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2tuwuxtro.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2dtxmrogw.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ictbmayg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2pphvmjud.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2yfkhvkmq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2thyonobg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2iwlgkmmt.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2vikbdbpa.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2hwxmjxfp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2idmbvsff.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2nfijivcw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2rexynlum.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tozyrddp.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ixjgkdpm.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ztmzucze.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2featojmv.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zjzlmouj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qnvcgprw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2rtdvrdkx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2cvwtgwez.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2neopgafs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2tmnzobhn.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2fmxmydzh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tcwamhas.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2myezykej.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2iljgsxnr.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2tvfxsqvp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2nrkfvuqa.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lztqlthv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jxxjkfyj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kugnvglv.html


<!-- 参考信息 -->