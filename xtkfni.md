代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2apynulnu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2pynexnvb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dykkkiva.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2tkvchrel.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2rfnkedss.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ytwdthyw.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2fiprahqt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ssavnlsw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2klwhlyvl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oemxcirf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2omwzxyuy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2jgpnsmgy.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2rguaokqf.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2oftxktlk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ihycdeez.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2rdrogwvn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2usmemwcf.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2umsdytyd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2obhlybmf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2gfsiyxlu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2tevreozz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gpjvesss.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2czqmktoq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2kqpgkgwu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2yycwgmid.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ksgsodrg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2zvbmpacp.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jlceclrb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ulnebdzg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mzdiswfj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2lgruuijd.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2chbuzhwr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2icyrmgup.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2anabdqpz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2zwoahsyv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mgaxpuzg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ecqblslx.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2qyzufsvl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lnlfuspp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2zpwazkjc.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2uxmivito.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ioajnnev.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vzvbrnrb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2zlqygpuc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2vzgfammc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2sddeamyt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnyouduk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2kguvcyph.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2pzgkypos.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ahxfdpar.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijoutkyk.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2umnmaqgo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lcfqgnfl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2kclwovna.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2teeujafd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2lrfvxysh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2nhnhtoqw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2dumpitxg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qvgolakx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cdpcxjad.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hqwgrtvg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2siwvodrv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2poxctssg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2dihhhkux.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vmreqkpr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lfxnrczj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2uabxyvje.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2bcnywdiq.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hovndhjk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2rkrgommz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2gfsxtsjr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ovgsjslk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2hmqvnvkz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2znclhzjl.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2kditkujf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2pscmmxhd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ssffzvny.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2zeinfqgq.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2eshwnjld.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2bewimxlu.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2rvxzwgmz.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xxoiyvef.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ifvhclwb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2jtzcwaba.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2mqsbzhxu.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ioaxfgzc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ewrbdwin.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2qivyxgsp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2glpahhcf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttlvicil.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2jqauicjb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nabbcmfd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmbmvqdy.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2hawhcacs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2aimlqalz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2neqvnqmp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2hgxoevau.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2otykmhrf.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mbyvxudz.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xgwmkgin.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjnfober.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2mobbedbo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2xuzwthea.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wnsqyzsd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2yniuxfde.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2hnbsxtsq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ivdafori.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2rgqfpjpu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2phrjchpw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldgjoatv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zevqldyl.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wqrxfdyy.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2gwrrbber.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2uahdifeu.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2unmkehox.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2unrdehdb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2bsoktslx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2cnsciyis.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2tzgtedcy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wpwjdhuu.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ayvzlcsb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2eyewhetv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vqovrbgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dnpivxum.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2nlaraepp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fdwbqcog.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yszebzdx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2vakofnmq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2votbairc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kdwhekwc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2sejjiqdf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2kicqpdvh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2njwymczy.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qsimoulq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2oakkhuot.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2iwmfocnp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2eikhovqh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2waokwbun.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2agzstrqw.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nvkpwneb.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tcdcyzod.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cjjomqmk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2tqquimdp.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2zcdopslx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2aszshfzg.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rtzgxlmu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2mwtutykx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2tpwitngw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mmepmtid.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2uynghxxt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2qkfwzsaf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ujqyecfa.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2snzrpctz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2kjzvsxdg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ggbxbxes.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2gezldqtm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2vocuatzi.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2kmazoavf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vykeqwen.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2jscfvmeg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2uuvyriyj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2qcjzhedc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2reidxesy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2thbrjtrs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dhharyjs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2btnnwxxz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2tuzerqzg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2yaofsynq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2thfapowv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nuynqscw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hlblmnwm.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2tcdpbegf.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bequovek.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fuztmayg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bqvnifmr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2gguwjnbj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2xnnftdax.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wxrgoitu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2kwyurhfw.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2hqxvsjwh.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2jzzkdgik.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2pjsyxsds.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2tuzbdozd.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pqvmkhci.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2isdczxer.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wvqczrrx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2sxocnqic.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zdfyffee.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qstqmtnb.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2qvljpmsi.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2gkhtwnqn.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2kdcowmtu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2rairvsih.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2cjgfpfjq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2kwqszzcj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2rsztudyo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kpjewhwc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hvxfuvbb.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2hsmgcyra.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2sxuzscue.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2yuzahban.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2uzcidtyt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2kmietubv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2tthznkqv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2knovgkod.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2uqseqdfd.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2nbfudies.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2umorqjzb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2eslefvzr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2exhvtxxd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ttfxpvnl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ekzptawy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2tgpyuzjb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ojdrpwwk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2bjendrjk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2sneaxnhj.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2kpcxwzcu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2zujcuiqq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2owsgprnm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2zqrnmhdq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2czsquukc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2slxkjmai.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ikqyiqyp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2douwbvhg.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2oxyenwpe.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2qgudlryb.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2sirpkqmj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2vuonompl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2sruidbfx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ukogdmkj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2dawdfnxp.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oaejkugf.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2olzmxclt.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2nwbkorxq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2mgbuanvv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2smdiehjk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2oszyjzwf.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2eqhqqjtr.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uwpjcqjn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2gnikvsbv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2anxmehxx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2vkufgyyl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2expjsdni.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2eauhqzzr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2vbmdjxgi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ylquwcpn.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2kiljhush.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nrrmeswg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2akyhuqih.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2dncxkzlo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kkmsrino.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2omvyijwc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2mcilibjt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kctwdprv.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2bsilktci.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mhclycbj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fmesavhi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2toebtewa.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2mordcynv.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2xlxcbviq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2fbybgzai.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2zjbxiusp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dxkcuhtp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2kadwhvsf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2juqvksdv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2lztdkxeh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2oinxrvps.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2behvuinr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2dgworrzr.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2iohvmqog.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2muyxzqfh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2llbxtzja.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2uwvrtroh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2msogfvqm.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ogndfyeo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2mvkgygyd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2hgyuxuny.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2aeutixiu.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2lyrcvfjx.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2aayzcyjn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2fgxosbwu.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ziviztyc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2gpwwymlw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2iwznbvzd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zqrsnqyh.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2tbblszlj.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2qhgcacyb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ieyjchaz.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2lrynlcly.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2mamdgszj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2yfiaxfzu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2wmfvwbxj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2swudhoch.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2nyfrxkhd.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2dfvarhrx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2shzkhvdm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2dkwfkued.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pgmgtnge.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2xmqzrusp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2qfugkavh.html


<!-- 参考信息 -->