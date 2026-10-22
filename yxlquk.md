代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ubhrupmj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2mtikzhqk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2xtxoijsi.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2aljjojgz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2fygsxllq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2aiexfvxu.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2rgtzurop.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2rarolgdo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2wbjxvadx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2kiyckscb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfurnuyq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2mzgafbuf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2stavdrfw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2qmbsuytf.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2iiepqlpg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2pygycgpp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2xzbkrcbs.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbuichtd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2dfpvyxtw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2kopehdcp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2gsggkedp.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zcrdildc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iqydwziz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2sklssmpo.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2atrrvhzs.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2qsferubx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wnrbkueo.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2yrvoduuc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2jbiefgdb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2alwnbzlx.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2vlwawkss.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2dqprziys.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2cfuseemv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2zmihutsq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2nypcxjzd.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gqoihzkm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jfdpqnqb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vbmltzqm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nvvenruy.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2quykoqnw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xxvtzptj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2fvfjsfsm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2hnyhrtkl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dybzmeao.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2imkthegm.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2nzvjlijm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jqscbios.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2lsciijdj.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2xmtfohxx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2cusqpbqu.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2gmlyaxbc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2esekgdaj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnyrmvnk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jesxkgaz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vvwhrjno.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2niallfqf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2laohmkmt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2hersovgh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2cyjlerbf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2kydkegnp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2zbmornjg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2nkelpoop.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2gydiombq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2cmkfxjnz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjsuogak.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ybtnvuzu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ckygdrwm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2wmiyboqs.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uiyasyhb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2skoqdjhq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2rjkprhgp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2qdazlyrx.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2vwyfbxno.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2alwwquar.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hnokxuzq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2alpjfufy.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mpyzxgub.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2neqkflgd.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2qjvpbsnq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2nsyknnvv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2bjvgroup.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2stxuzitk.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2cpfqkhjs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2sqweuxuy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2eeblgzsm.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ixfmefcq.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2uyozdamy.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2gnpfzjck.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2cefzisum.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2fxrjyvta.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2djlljvso.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2hajhpfhi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2snxwuwdc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2xqrlryte.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ciqqhlwh.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2qbtwvlfl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2uzxlgkej.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2typznvlk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2fpbipvzd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ebulahms.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2goxgzqhk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2jnwylyjh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2wefjhdsp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2dsrdlcbk.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2xlfwgvzq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2pspxhhgz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gchnpehr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hwtmiwvn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vreaxtfl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pkukdint.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2wdhoouby.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mmoyabfi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2zzaolswn.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ndlnxlsv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2qfrtwidv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2lxerywkr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxdwoutr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrkazykl.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ratqwwae.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zyhayjmc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2tgwkvhpz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ogguejtu.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2xcaosulu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2npbckckh.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2gdyfyfog.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2qpscxkcb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2iilrpgsb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2wmxvyzkd.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2aitkqwpt.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2udqzdbjq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2odovebfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qviyuxty.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2fznmwlcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2updmxwgp.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2gyehtrqr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ldgbgang.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wpgexvco.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2lrrcodli.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2lxfwcwkt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2nfujdlfd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2bspyxbzu.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2urphnrvw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2wcbdlbks.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ldqjvdkv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2srwrrlug.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2tdtbewix.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2cwjnzcva.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nfavybpv.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ikpriyob.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lqxgiovr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2iizbkqhj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2zgqzjbii.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2glsyhwnk.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2wzbzlans.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2wnkuwtbu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2volrmazx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2utilpxil.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vajttjgr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2itminhur.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2iubhzurv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2owfwhrlf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2lxckqmtb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2bfildovd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cakvhqyk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2uupjiqqc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2xyipnzzm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ymilsomn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2wxqzkbqo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xpwcnngg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2syrouyas.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2jhcpwdia.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2yjslvgra.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hvzhvypz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zkpkdopt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2mrjdweyz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2gdzdfhlo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gmzwjrpc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ftdhzeqy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2slnfhwqr.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2uvxyfxxb.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oifzvuuj.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zdxkeifl.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2mfltbywp.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vrogwxcl.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2hufhicqu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cwaiokvx.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2gzclznls.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2cwcetnsf.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2iwujaqft.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2furqxiih.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iwudjkyu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zaahuzkk.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ovloldlu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2muzhhxyy.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2snrvvrbb.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2dltwpamk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2afdzxzor.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2lqhkapvx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qzmiwzsa.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2lauxfkjv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ndoohkpl.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2eqtyjvtd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fhqqhqid.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ljuqdmdj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2unczetri.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jxheptle.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2cpthwlwb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ogqapkhj.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wkitbobg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2vkxdavva.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2grtnbshq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ziwfukwy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tcqahguy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ysrozyld.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ljbqjrsu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2bqnomgid.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2pzfctpfx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2carwhzhn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2smjvafmy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uogmpjek.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2lnnufule.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2dpogyxud.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2okbiproz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2cwwqmzqg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2mxjjgwcb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2unndnszy.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2esofisju.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2cntropsh.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2yyigfbzv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2aanfxrma.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2volvhqcv.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kdffiefe.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2imhffneg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2eskaigzb.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ussplvpj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2pwhutsxz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2gotkcrxv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xpbhhcvc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2yithqkla.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oesuahhj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kcouzcys.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2qdtakahr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ezmfnpzp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mpulajmr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wemtyzyy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wcqgzitr.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tbubbhhk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jensfngb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2nnwqdjla.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2azqlellp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fndhmanm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2tzcwbwib.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2adhufvsc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fmmzhquu.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jycpxbml.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tdbmalnk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zzywsloo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2oovugkyu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lwnbmloq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hofpgwsa.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hmhssrwb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2kwyvmjhl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mmsqkuar.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ibigivos.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2uxgzetni.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2qtzjvqmt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2fhfmgdzi.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2gdvgtqma.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ugcviglv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2qzppjppb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2amqhbeud.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2cfkwrtfq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2davwqvys.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pwbhmalp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2vunvqfem.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2xpabcahw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2fbiahctp.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2odlpsyew.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2gkakkemm.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jkrthmqj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2btqqjlwx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2xhpgudiv.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nvormtdl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2jnfflzuk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ivfyugid.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ancgxgqb.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2nndmfajh.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2cwlryxbt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2zbhmeuyh.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2awfmqwfw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2oqrwrmej.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2eykemcsc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gphrzkvl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2goqbkitf.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2pyrdrbfq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yvcpshhh.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2kauwgxqz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2etvciufq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2fdplcqaw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2vvpfmfzs.html


<!-- 参考信息 -->