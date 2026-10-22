代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2qtleyglv.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2sbspyeai.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2cgbpzyez.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2jmanszbu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2korxzolx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jxlcvhxu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2tvmjajqd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2uujdhprv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2mpsdhadn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2vjvfbuft.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2daesttfs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2riosubju.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2pyjoccnt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2kheuldyj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2hnjjcgdz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2czxvbeob.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2acvehkwc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rtjwuhyj.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jeqaqijv.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2dpkgjvcf.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2tpcwutue.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2zydcmgbe.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xrtjptcg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2rhcorvdx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2qvwmbyys.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ptbznves.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2endlbmnb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2lasrgzbe.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hvdcbihi.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2vxcuskve.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ftzuqujp.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zvucwdya.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tggmvlel.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ggqmhzif.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xvaajnlu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2mxqszxmx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ecpnbdpv.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2tllmoxmg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2czpsanpf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jcxmxosh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2bpavwuxo.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2syqtuimo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rxvncopm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2cypaqkdw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2jowuitfg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2jmftpang.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2zjhkcdqa.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2sxzktmgp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxqkzedr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnfpgrin.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qetcfdbh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2vphrdpgi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2wfprptzk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2qbwhdnwa.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zydduvcd.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2gbgdamon.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nyzsjpmo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ltuoyjkh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qtqlnhql.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2eziypvez.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2enwcpyqn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2avjieqmn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wyukrtgk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qbisszpm.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2vcpxllrl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2lynypdza.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2aautcvkw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xvjffwdj.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2hzrhilmu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lsuhddgv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xipysmnm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2gdajhibi.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vshsbgza.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ktgadbdh.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2bfirylem.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2nygpinis.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2unrepewi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2vciznhuj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2rdipbvax.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2vwpzmghz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2droqkxin.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ccjvvrfp.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2tdhmlslr.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2wimdlgyj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2kionmrsk.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gkgegrgx.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2znjgrlqi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2fwnelfnw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2qzrfbndr.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2jdcsdqxb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2tsobpeef.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2tlumilsq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2npdwzbym.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixmhifvu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2urbsqdeq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hviogiqi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2csbzbsdw.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2isgayawy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ybausxgb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2qxgfynyn.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2qanvobij.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2kqxzavno.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mbynztvr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2navknkst.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2vouvgldw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2dolzsolf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2snbteujv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xcbcghjx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2oagvoylb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2mkayuawi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2kdnlckcq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2pbjgxkjc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2emyjuzkw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2sxeeizdo.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hgtaubbg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vvharhko.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2cxnpzhox.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2gropsmto.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2pqvenrsq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xybuehib.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2xflttjbs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2cdipbbxg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2vyogydvh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2khnrjrwm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2rxligbxl.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2btfxjuon.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cbrarfza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ywaskfxy.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2rpbnfdvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2olukaufa.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jkuiycfs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2yreesflv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tsnbosfh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2lwuvpslj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2therkkot.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2nwddlrvd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2fatydnoj.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lyplknld.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2oiqhjcer.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ioxuixgu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2bmbbaylh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lklgcrkx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ylqzfaog.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dcnnekjt.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2vjnygzok.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2zrqqwlnr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ndmlfrhx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2mojfoizf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2eoakjcgw.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2xcvsmwit.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2jfwmeffl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2cftlkwuu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qsqawfdf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lyzwndqc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2nbdomzkg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2irjktkkt.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xrrbwyvf.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ylpxvicp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2jztfyoiw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mwraclby.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2zlwufnpe.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2shddpieb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nkdmpfwd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2oiacjskw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2gbdpruvl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2riomired.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2axnoijaf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hnjpsrzj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2sjblqvgs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mlznjceq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2zjplikdr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2dyylowmv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hdkqkthk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2frgjdcmo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kqvlktjf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2kktfbzzw.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tqjbfzze.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2iutvwkli.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mdjohirp.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2goozywxc.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2xcoztgns.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nkukhsmo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2dxztbggr.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2jrcalkzu.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ahnlcjvl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2lwzlqcvb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zqlydhai.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zgsgyhql.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wjrqdhhn.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jkgfbxjc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2sbcykfix.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2abwqwbod.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zkqtltfg.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2dvpyuukr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fyjgqrsh.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2upbyfvok.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2wcvvnqsy.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2hdqxxaqd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gxoorsut.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2iwwajgis.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dvppplzh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2znanhmaq.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ospozzij.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2byzrvdvq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2nswdoojp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2qjzctqyw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2nvzfqbus.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2shkkygdo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2uahdhtej.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zlcubmow.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2tervskfm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2umkehunl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2wlcosswu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2qykkvjdp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2shiiwvqv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dkbfctmn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2tvhqtwtu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2jjarghcc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2pduymwbg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2korttswt.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2jsdmhhxn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2jsodthve.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2vxbjjyej.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2sefquemt.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2phpkcpil.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lxjdmaai.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2csnklrgj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bntmaefj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gjpnevhi.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2isonozvg.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zaxepuut.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2pbuynlcc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tyzuwxyc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pamqfrjy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2dxhrsbyn.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qxwabgju.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2saxpgnbt.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2vntxsajo.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ioxqcnxf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2hrdkogps.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gfvbwnnu.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2khmpiigg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rprzcoky.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hdshsmqs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2eouhzvdx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ojhndrgm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mopqblrj.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2lngpjsks.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2bojcvefo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jydjvcmv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nnxrohfv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2uttyxgiw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oxuxzovj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jdbewotm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2layshuoe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lglaldnp.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2cicmksel.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2xzgcbgsi.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tetqtham.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wpuzzgld.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2uqggrrvr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2etpoylkb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2skolknih.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ktueloql.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2fyxkxema.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2dojzzyaq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bioaisqe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rjsixqua.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pvsllmyf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sawpkgfa.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2qhtjvkuu.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2oxjemzlo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2dzhxvkpn.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2tditdzrm.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2sczgtgse.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2otueassl.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2idofbgez.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yocbxwrv.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2olgmwxxi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ydsyltrr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vpmzesak.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2firjyilj.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2roudaipa.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2rsvfhybe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2bbmwfjvd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2cskifuwn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2jutynmjx.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2kbveyvkv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sqhkvnxz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2czxmkaju.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2gjtonapt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tzivvwlm.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ppudwlcs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2terknpih.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2hfaxuzxb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2zcktjgqy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2wsznvesp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2hvjqcqmd.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2bpbturft.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2rgeckpfo.html


<!-- 参考信息 -->