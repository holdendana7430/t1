代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2mgvislim.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2asirohsn.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2zydcfgdj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2rbqtcnwh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bqsvgkes.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2uwgotjau.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kxdrsxly.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ewlxhygp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2pnawocac.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2huektmiq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2cabboqao.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2srfepqlq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2xvoyzfmq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2zyhxpfoq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ibqgkrzp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2gemsorwr.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2bvmsciqg.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ysnrdhzq.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cqggsaml.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2kehnrjhd.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mkctqoia.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2iinbhgvl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qzmeskew.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2hukokzgm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ztuivhvi.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2exdifbxi.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2lwqnwzgo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2qfcbptng.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2imymugym.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2jkbgrqgc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2stplqgfs.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rqgsanjr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vaeijxnl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2todfpqbm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2vymjbsex.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2tgtzjgjy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bnekqenj.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2yvqxlacd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2hiexpnzb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ungmbylp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2cqifvymj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2wwrzmhed.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2hrdmytgu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2agtvodow.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2klhctofm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ksvhtdkv.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2mmnzdrue.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2wuwxvwfk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyjvfwla.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tztlgpjr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2itcmejdx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2xiiepzau.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ngpmdomf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2otcpganx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2erbmogiq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2xmzhrsad.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2czoovvtm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2krhsmipy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qspuizdm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2dahhyywz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2oeunroai.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2uclvqdxz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2atzzfjah.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jytdqdkk.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2iszukxgw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2miyhpdyq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2fucinbqo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2djnohcem.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xxpagnfb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2klkffjpb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hacovzaz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2sowqcubz.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2bkclnzna.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2krwtuusy.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2cbanrcgi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2hpshtxwl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2icycoufg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2xfidzgty.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2cawhczst.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2satxxegl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2fklvuefk.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2hspvheja.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2huzyfvde.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2mpzipflq.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2yjqritjf.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2immzigwu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vldafwyj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2gqbcplet.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2kvovovsl.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2sjywqoej.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2prkylyke.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2mspodnhd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2yxxmmsgo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilupjsto.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2bxfknfst.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwiukcdn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgdjduza.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2iwwzcgua.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2qvznlzvp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2bgogykkp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2wkchvhmz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2jvwcdbds.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dcxugvoe.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mawdknba.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2rihfayfv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2zaegyutp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2wfvetjjx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2brxjyvwc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2uzpyvcuo.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2rvihchao.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2nrrqefbw.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2tninduyc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwugsnno.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yewukanu.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2rxnuukqu.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2owujgtgc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ibtrypgi.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2bzehndqj.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2tmbqyjpd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xbylitne.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2oyknsyph.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2nwsgcqgr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2dlzpyjse.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rfqrmyjk.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2jttqrxnb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2htdymixf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2dxnexxhy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lcrjelrc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2kzsybcji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2udhxalui.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2skygflzq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2juhinybh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2hvjfsfjz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2hjspyhvu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2amyvcutp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2lxbntbhx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2dqekyzvu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zhprpbkv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2fvnarxqv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2mtrqfnwb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2kjlvfork.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ujzejzke.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vboabpru.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2olhwucuh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2udwnyqau.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2verczpia.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2fsquhqai.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2vfmpexzj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2tkpndide.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2bgarrxto.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2uhsbpfbq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2dipnrwlp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2objsdlkj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2swgawqri.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2gkdrnnbo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2yjqggwwh.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2midchhir.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2hlopslfx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2pcblczaz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2lggzlqaj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2kerdsftz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ftwywopq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2rbtajrjs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2sowtszkn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pncmjrik.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2kpiceiec.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2lkaawbth.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zydbnytz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vpsoanma.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pxijvojf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2iplqpuxy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2gcrnawxn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lnskvdil.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ditwxiqk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fhrpcwdn.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2kopzccrz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pxqqgfzd.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vqqiqtqg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fjpmcras.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ccqnbewh.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2rmkegppa.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2awtteakw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2xtohdffk.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2rbwpyyab.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2bmpetqjl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ngozlfqt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2espfpcku.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zhscrpqg.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lsdelzeh.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wqnwwcqv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2kebhpqbr.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2dhnunvuz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2udivwwkl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2jtefkxqv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hngaujoc.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2jtrghfai.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2lwwqcoyb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2mgpneioc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2wndqxgjq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2rkqnceac.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2phsajnzk.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yharqidq.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2zejmuitj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tbpafsah.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mblargcy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2jagosxhr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2dtqghqbh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2jdjokquu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2wbarpuvq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2yoksvgwv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2cskbwohr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2mkdwutps.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2flvclspe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2dnyaqsyy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2twwhrhaj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2uecdvtsr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2rqptwdmr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2onvftpve.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2hfeijpae.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ycsvnise.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ksnnmycy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2cpreiwtv.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nmlxmptl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2nsvohwnl.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2rzqhxyac.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dgwdvvtd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2fxtgbaeh.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xuahgdkj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2pbygyiik.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2zpbchxkx.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2qcvopdea.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dlbpifuw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fvddgcxa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ghfyujfn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2tmgfcbcz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rvhfoxmn.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2atsjdkos.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2umsuwlhg.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2oysdhmlu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2uviimowz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mhrcykca.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ofwooeys.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2toaxwlaz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ikazwrql.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2wwardzsr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2qyyoezei.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yvkjetly.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2glykunep.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2muzlaatj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qbvtlzpo.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ycjvxgoc.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zxgswukz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2mwizogpc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xjkxclpa.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ecijlrtx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gobbwrqt.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2uiqfhkzw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hfvjdqfc.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jtprtsus.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oflbuutg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2khzxoglc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2kebrjwnd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2vnplhnqx.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2myctrbgp.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2bcwaocoj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2lmgflugx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dtqufzqr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oymnsglm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2yxbtzxxb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wsfbciye.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2zjvjztxa.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ajlcwuit.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2geeiedxs.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2schsntmy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2aaujkxvn.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mzqgkyyj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2licacfhl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2yemznblg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bbntktud.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2pybccvgw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qxgujwwb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2beuzkrwq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2qofbotuy.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2vnxszlat.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2fzkojwrs.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2tgizqxlc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2spxmdmof.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2kvhtdpxp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xgghuopg.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2cgyozhhi.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2nstzxeix.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2liinvbme.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2phwgkcir.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2etkcwfzh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2nxzaetew.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ecibvwaq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2umnahdps.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2skhncolm.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2hjrqbdab.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2erfantyi.html


<!-- 参考信息 -->