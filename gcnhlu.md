代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iwnngvek.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2pltvethw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cgaqqmqh.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fnlrsnhn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qytljxtr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bijsbzux.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wooxjpvy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cpzsygnr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cunwomen.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2apalrdwx.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2axoxynme.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cucjdmyy.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2qfegomby.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2mngfxego.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2plkpvvmp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2favsftxf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajgtlett.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2nsgvdfaa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2xuspvael.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2rtzariwo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2yzgeqqpe.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2gtrncrvu.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2tbdixipm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2gqwaddes.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2oqdxydyt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2svaddxlh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcezndzf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2wbfhbcfz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2etlpmduq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2bdantpzs.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2lmkwbhbk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2fkujsafm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ulbkwuky.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2isozohqj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2yuerpmgb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ajzyimyp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2kzhfivrl.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vqcinhmj.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bishizia.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2fukfhcxd.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2qvvilybf.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2mdvdkdws.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ffpviheq.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2rinevvlo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2cozbffou.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ofgemjut.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2gawwckfa.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2uobbdfqd.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2fmwqyrla.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2nwplbkex.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2tlagpbdt.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2akfxpqlr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cagulaki.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ihmchton.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zisupuen.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2vweybmnd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rclmscvd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2qdacncxs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2glyhdmhh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2exgnslnv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2wstqnist.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2cqgftvel.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gwzhkfpy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2qjuteszt.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2gldgeoqp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2obqrejao.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2eetkoulk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2lwpjwhui.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ebdqwauw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkrkuowi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ilwaihul.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2gccdutev.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2aczjrqhj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2hgcxnhqs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2iowsalyj.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2sgzummxf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dknmwsbv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vnvwucyu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2clavjtmo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nstrcoit.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2bmtkbxfq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2fbpquyps.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2junoqwls.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pfbfwxvu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2dnwuqptq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2dnrkfqqp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2nzmefvsg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lmlkzlob.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2cpexglyc.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hadnombb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kfnmeama.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ozhzjxat.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cfgqbfag.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2idixxxtk.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2gauqbpji.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ssbkigcx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2pbxduvko.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2npvpqjoh.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2mssjyizf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2zoqdhrry.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2zogpqjpk.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2lqvvnmlq.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ficdpelu.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2bpraruii.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2tiawmmfm.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lzhumxuu.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zxerfeju.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2zplgnukt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2zibpyzrj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2gjehgniy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2pktbvxnq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2trnzkjfr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2pejqxqvt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gkvgevgl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2vdbrumbd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tnsosoki.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2spzlpwcg.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2nljgocwp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2xmkziibz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2lfexunlt.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ovdwnmdb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2jtupocsr.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2glyojczg.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pwykreyp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2miwtksib.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dedpzqli.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2jgwzfhph.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hjdtxnih.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2fhvnscpu.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2qagiputs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2gphyhrgw.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2fntusrhg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmmwzvcj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdhqtywa.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2pdwvbugu.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jlyujnos.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2imoutdaz.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2aglrftvd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2vfitrnqp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ckiifsyx.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2bnisnxyg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2qzxfvmoi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2vtdndvew.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2drjqjowy.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2spnsqtvu.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2likagouq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2suhnnden.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mzyhlrar.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2xhvusbez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nyyongxp.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jylqywlg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2vrbngore.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jbnzglwn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dekbsedz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2djjcaxln.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2pibcizxh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2lipzaevm.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2jiktzmto.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2tapyeqzn.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2vxvvigbf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2tgzxwhyw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2hlrefrvp.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nsopdpeg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gpdumuoh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rmwyqesw.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lenpeakj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2blqmhjaj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2mlwdxzsb.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2mwykvrju.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ljvltfdx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2tyalnbkq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2tephboom.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kqwvzbju.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zajnbnsp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2kqvafvll.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2qutqludk.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ymtckksb.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2sscnkubq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2hbwkeztr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2irmsdptm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2uzdjixhe.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ggcnjpod.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ctlsjkgx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2enbptlaw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oyxlgldj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2nldnuznu.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2xrffruvy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2azlqwpyd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mhfsgqrw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wggmbhkg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2mruvjanq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2braylywt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ddfyhbpl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vwqtawsj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cxphiooo.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bccwpwpn.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vqrpebla.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vraicykm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wfknnipo.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2agyulxoz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2fbvwlugq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fcnahxrt.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2lfldjmpe.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2twjsqgbl.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2vsuvvqrm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2dujklxzq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2zemsqbmt.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rkktzkcj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hswugert.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wyikdgjc.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2wfkibppy.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ktabcrgg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qvqgzjcf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2yziyonzo.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2bcywsrtz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2vtizcaoj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ikmuqfjl.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2tlmliodd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2znsfstgk.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2wzokvzdc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2krgodkhg.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uoruzmca.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2nzvmvbxn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2dfxbymei.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2qwmupaoc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2rxjxlyde.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2jsvwexaw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2enadfmmj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ixqvjmdb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jxfpryvi.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2jgyzaoed.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2jfytmrjv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ngjsjmpi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2velsfoda.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2sslxepoq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zghelsxy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ufxzwddv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ywrkuxsm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ijytjqtk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2qmolnwje.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2tnrudkgp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2tfsforrv.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2auzjubnb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2jlmvrsxf.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2fvdhevhs.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hvjwxxxz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mkccopox.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rabvghbk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2sahxhpmp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2rcnsqpni.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2mvobjjxe.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2vrvrizfw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mhbnmpoy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2louiuyew.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2waayjqqb.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ymcjouol.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2yczfpbst.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2jpidjmig.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2veponiiu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2bonusoyc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2czrdooje.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2dsnqdbho.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ahqbfnwy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kcbkdslh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2unhlyvdo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2zwbpidvq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gkkfbbpk.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2pidlrhhy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2lvmqofiu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2pysypfnp.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ahfaksse.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2gbrmsknp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2xpapgebx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2obxxkcrx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nrdqayul.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2aboyffgs.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fiyoecto.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ivrnjibo.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2nusqjusv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bmhgppbg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xjpwcnia.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2cqkdoalw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2rmdlpqqm.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2arsrcrws.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wutxtrld.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2duzgfqxt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hwbmjwjn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jnunydwd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dsqgnumc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2knbezqxb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2rjqqqyfo.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2qewrxeav.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vufkehev.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2vawriqfx.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xnwjzxki.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gxjfltyz.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2efjexlst.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2mobthwta.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vuaqeegs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2xfcnsjvz.html


<!-- 参考信息 -->