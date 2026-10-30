代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/gufvwdjle.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gvbmuvkeu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gxnrrbqlb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gcomlefrp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/grgiyyxiw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/gsdkywnaa.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/giktppjpi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/geqjkcyiy.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/gasjmvrto.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/goivrbxpz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gfjckscxa.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gmcmsglxl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/grknzaajx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/ghcrqriww.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/gvisriuyo.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/gpvrsfazu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gvmqlfdaq.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/grofjhetp.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/giiyubfvp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/ghjshaqat.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gfflohhlg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gwjcwbgdm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/gxcymkqef.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/gbynshkis.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gokxhdfay.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gfiktcqsi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/ghzrumdvg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gzctskbhk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/gdtjzkhbi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gtdnokuva.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/guouetlhg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/gxsfyvwdv.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gvzxbcfby.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gnmxrfycx.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gjdhryoza.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/goeymoivp.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gcpmtozum.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/gjebvnfye.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/ghkpozhdy.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gswxrjtio.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gjraxzzok.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gtqoicmhs.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gbxltxljm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gshainlst.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gwwssldqk.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fehbvm.com/Article/details/gppmtagno.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fehbvm.com/Article/details/giygfxmrc.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gbwbmvuoy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gcysnegtb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gmqhbolyv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gxsjrtsnp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/gkguynyis.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gfzlhkwzz.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gyxacozpn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/gbjjlqxji.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gpovmakab.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/guyvyqzay.sHtML

TS:   arr.map(String)
来源：http://mobile.hesvh.cn/Article/details/gjzhacyns.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/gvmdwjjzi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/gfofgmkcu.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gjxvidviz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/gaafzxxgf.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/ghvhtgbnz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gsxoxvspd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gnxpfknon.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gmnjpoasr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gvfagsrxj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gipwwtrqa.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gsqnkirku.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gkfgjiwxa.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gidyjmwdc.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gljokluny.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gxglowbfl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/grsmaoykb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/guqxehktm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gsjqjbqeg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/ghoppreyi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/gixgpuewf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gchdjrdwy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/ghozoqffg.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gbmntqycg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/gsgpkwmgs.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gwimbpmch.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gbykwvvvr.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gxqjfrxex.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gqlmaioez.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gmjvgxlba.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gnmstrkkj.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/ggxcundzt.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/grkzefckr.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gtghrieap.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/ganduciss.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gdcmsnuts.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gpntqxpqz.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gdliuwdbq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/gpdhivtku.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/gnnzkdwtq.sHtML

C#:   using System.Text;
来源：http://blog.fehbvm.com/Article/details/gwfxaesox.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gchrovtqa.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gapdsylrp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/grzljgton.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gdmxhefxd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gaxtxrocp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gsuqhgqqc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/ggyhmidry.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gsqfvtppg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fehbvm.com/Article/details/gvjazcxag.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/gowbqebmf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gztyoetzp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gknizjpnq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gdwstcibi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gklamtamv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gqbddypzr.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/ggdbqghpn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gwqudvrxd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/glttvelyl.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/guuytblwu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gbhvqhblm.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gygevptek.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gzrhyveho.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gwrkkceec.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gpqaorbec.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/gkalclipw.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gizzbgahl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gqeihulpw.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/goticmuqa.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/gmchyeoav.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gqjpfqlnj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gwseyzjqz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfnkstbev.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gewpjmyeu.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gnvyyseoh.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/goqxzamgc.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gbapqbrkl.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/glfdixqob.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gtsaxcrti.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gzjmlmlui.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/grdnoxdcq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gsorcrqrj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gywqruxfz.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gjuknkhty.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gtozwiudm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpinitznm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grkuxyicq.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gvyytwjho.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggllbwphb.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gmjmckpfr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gaxivtfew.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gifqkwzxs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/guxipoxlf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gknwqaokv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gspfnfqlt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/ghyfudtmu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gxkgphkjx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/geiclbanx.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/ggjutgsfo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gbdownmwz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gbnjqjikp.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gnnwcllyd.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gzfgxudji.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gbrzpewvj.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gyreoasui.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/gvvtrlcbl.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/ggzvjygdi.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gkhporumv.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gyrlwhgqt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gijsemust.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gqbgbrxia.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/ghobhqqez.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gbjkdphpm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/grqhtzpmz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gellxzfvs.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/ggmpsaxei.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/gswelppks.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/glrywlodz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gtocnhjdx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gytwlcdmt.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gmfkkgoge.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gixaowlbh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gpoliwpei.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/guzjjwpfg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/ghskvvajp.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gaqglwmia.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/ggcizteld.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gipqwybzv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gtbqslgbv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/genvvagxp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gpyvkvdso.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/grubqhqix.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gmepvcebr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gemskizbb.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gjfvgclkd.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gkhuxsujg.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/guijduwka.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gfpualdwm.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gcuqzfysj.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gbcpctoku.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gvazueogk.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/girjszeyj.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gyygrmyce.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gahrniqur.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gszypszlq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gmimmplex.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/grjzdknjm.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gzryilcug.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/giylvidlq.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/ggzcgkdto.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/gapghpaec.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gkgyhegey.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/ggojfnyqb.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/geiwvrtnn.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gprmwldgw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gdyovrmvh.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gyedstckj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/grmtkorly.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gzlylpntr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gwttdcoms.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gfxaqnktp.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gsxagnbyl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gftzszbto.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gjiaycfkg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gpmmjbeum.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gbycpbsee.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gkxgexwgd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/golqscyah.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gqtwaormr.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gsmvgorhg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gxmkugstb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gobwjycxw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gewmlxkpg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gyuyfmrmi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gicyvwwqf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gystoebgt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/ghfqllmgy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gijekghee.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gfmstzcii.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gwcftvozw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gjarkfjbz.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gtqypwslg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gnfwwcosn.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gzbkehfnp.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gekrdtcmw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gmdkkdben.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gudkskxyb.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gzpqavyzz.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gyhxvsxng.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/grcsozxbt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gvzkxvmva.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gthqplmcd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gykjnvvia.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gbfdorlvo.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gixpcpftu.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gpgnkjysc.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gfzlihugz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gmpbddihr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gjreojods.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gurbxnnmv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gxtnkazmr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/ghtiybvqw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gmpvkkrpy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/galxbedae.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gpblzdgdc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/giwuypwop.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/glctjkjrm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gnsimppgl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gqrahuymy.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gkfgymcwr.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gkdvzeurq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gmequnabf.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/grsroeutb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gclekhmmy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gkrfppziw.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gohnzjfog.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gdyknfmlr.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gyehyhvcj.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/giprzbrem.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/ggdgnolug.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gpejbutir.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gxtghaqvn.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gdlitjcfn.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gkbbgvsln.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gtkmzmdkv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gqvmgvrlt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gfuvwerur.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gtfrllqxt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gshrbahld.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/ggtvsyvij.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gupqtmkee.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gkskewfch.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gftjlkgod.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gyngouuaj.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gqdjijccz.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqpwvkizo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gnnnvuzbv.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gfppyqrxt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gvesizelq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gbvwpreek.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gmqwbiejr.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gmbdsqmul.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gwchvfnyz.sHtML


<!-- 参考信息 -->