代发 wailian999

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2wuwfaczt.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2wskrhpjw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2sypcvama.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrbvgiyc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmigaxfx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2fryjtrjp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2hdgdsxog.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2xrgkfnyv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2xyexorvu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2betqobqx.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2hydbsnee.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2xnuafckg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2uncjudfh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2yuuwnmoc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ivwwahlb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2iieveipr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2kxlctwmi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2jnpjurks.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ahmvssyt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2glpyamkh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ihislikg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2zfwqtkpc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jmbqdrjv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2mblkkfxe.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2woasthux.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uaansmvl.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fpgaxief.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2xeupayil.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gcaaehaj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2jehyumka.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2jzovjliw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2oboxhivn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ayczqsxj.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fpbiidwi.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2nagomuyu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2cglkncju.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2dpgspazn.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2quawndwe.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2oeetupux.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2sldokvla.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2arhchunb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2nimytsth.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2qqagvwyq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ysuokvjd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zgdyfefa.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2itxdpauh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2dnuxocbs.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jwzqewbf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2mqhgxaza.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2viphxkhn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hzjnlelz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ocroxwdn.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2tgmdihba.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2jkmtilfp.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2myakgbra.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2gygmlpte.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2lskzifuw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ayakvnxh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtfavmoh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2mfqobtrm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2tbiahcua.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2inpjmnot.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewspjfjb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2lvxntbrm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ohdvlvpp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2lojebjpe.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2kszatyva.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hnscigdr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2vuggpnua.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2qjotsvel.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oocvyium.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2nahrenxl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2iczinuqs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2puoetjia.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2keaxevcc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tzjzqlhy.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ignljhdh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wnkgkoif.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rhxiwjbz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2pkdkrgnu.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pdulpfpc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2aezxdyvz.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2myhjsfcm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2kdjeoqsn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2cxakvcig.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ahyvjtws.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2pfgjemaf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2vontiraa.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2sbmpevik.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2lpyloszd.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2pqafhjfg.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2jnnnlvjr.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2gjplfpwy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2okdhorjp.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vhxssqvw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2rdnufkqw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2kzqxdbah.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2tcabfwut.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xgflrtmj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2smynzfyv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2nshokyqi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xatfbhaf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2vumiatyf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyvhrbud.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uisqpgzj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2axmbysxn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ksqfpbsy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2iyleovah.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2xzyuobvq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2wumvvfwq.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2clmtkotf.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tzscqjju.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ihjuibdm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2zdmchduy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2mkfvhaiz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tbwamkbq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2vouurftq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2uxatpvic.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2cqwcrwiu.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jrtqlptj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jpiodlfs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zlridwxa.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2niitcnwj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2izpvulgj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2isvhokzu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2bxizoybi.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2bbbjisox.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2asjtijyw.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2zvqvzohc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2kpqhfmea.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2fapvpewi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tfyooenl.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2gjsbspru.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2gukscpkp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2sjdsazfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ivhsgmuj.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2kiqlauez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqzlodmi.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dzayefhb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2wksddgyo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mslucsji.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jjdnarrk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2qbgygsyh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ttrmxvxl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2koozvscv.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2nnyvpusj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2vqqlniek.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ztsyqatj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2bufbbgng.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2pqiwblkx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2puyxcgiz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qadtmzay.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2dbjyxtdn.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2lsgkjgvg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2bhaxdtfu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tsybcexr.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2vxwivirz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2crjwmkfa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2xfykdnlm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2wtpsudzh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gnaityph.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lcragnce.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ojinxczy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2llnndpkc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2anqvapvh.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2jmehqmwn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ozmadrsf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2rszwsqdo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2svahaumm.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2godkpwgj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ovpcnjjo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2nexnpfmq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qubbktxz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ptypdznr.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2esnogeep.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2behbfbnu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2segnzyno.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fqfypjkl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2dgsbzaqw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ctkhqddb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cadaebdf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fcbujvjt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2aedbqwrz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2zygvmsbz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2peiiapxx.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2gzxkwjck.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2bukphacx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2xfswhnht.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ixvlxpqq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dccgscsi.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mmponqtr.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2fdcilotp.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2xppslzvn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2qxguqngv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pvowcisz.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kywvjxul.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mfxnmqsn.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bhxzqhyo.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2waajopyg.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2hrkcoidw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dlocyhbm.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2fwtsvzpj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lopvswfe.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2cfhvoulr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2aknpnwmf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2dzeysbie.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pblttdkj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ljqwxuhy.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2qojitskk.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fxejkwiv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2dsjllmhb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2eahckpot.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2djwksibs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2mwhzowny.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2jyznlelg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2anvfqmgx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mkjdnrjg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xuaqmwjq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2vueycelk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2qsgyzddj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bbcaqbcr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xrimesbl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ycypmrle.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2gdznfwgc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2gjpffybm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2dybclgpg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2yalzatud.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2lndcifhc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2mwpbjuap.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2kbigepek.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tfkdyasr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2nnqrxrmw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2dfhotmyf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2imqfybyv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aulwvqnm.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2kaodzywk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2yhfqjzzx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ffcstuih.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2rxaorqpj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iknizucz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jgpvmkjb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2jsgkrccr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ygjjbsdc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vqorkbou.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2vwixdqsr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2qezqflsr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ovbfxknm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2gvxekfug.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2myexnlra.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cehyjqjj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hwcaanxb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iehepaoi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2hadtjrcv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2tesyhmog.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yqpbouac.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2aqqsywsm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2yugrcnnv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lmhizwek.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2yeaprqan.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2toqkrshu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2rwxzvvpc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2pcafoefy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2beywmrvm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ekybypho.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xmfyyghs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uwzngpdd.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sizlbfio.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ohulhhmt.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lodanbhj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ymokuieh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2uzqxhwqs.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ywduojia.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iltxlase.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2bqxwiatv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2efbznfox.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2efbahpwd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ckqisbvk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tpmobtnb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2xronhyzd.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2rpdzdtcq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qalxuikn.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2axfyqajq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2pwsjiguf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2snlrngwg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2nmrbpljy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ovgnoeoq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2amxnsdnw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2squlpnza.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mnwhyarv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ppiaryei.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2tfdzcsvv.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2atjttiho.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2bzlzjajl.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2wwlyefus.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2zaaidxfa.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2kqkklqac.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dvzhxtie.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jscdyrid.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2xcosymng.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qpmjmpuo.html


<!-- 参考信息 -->