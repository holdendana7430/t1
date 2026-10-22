代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2uxuyomrt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2qehzobrh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2pfeftdkl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2pspjqfyp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2hcntexpu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwtwscny.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2wcfbydee.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2unyiqohf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2dxoycqqs.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rytjcbyd.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kiyfhttp.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2cnrindjs.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2jhntvmqy.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2kdhrpjnw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2nvxreqjm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2dbzukxpc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ekriwhek.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lwjqtnki.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bgqxljwx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2bxxqhsmv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2tuglebpl.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2frjspnvj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2gxoxrimk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qeoybtwe.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pdexeqgh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fjzwptji.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ciueigad.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2bpgbtlva.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nwfnwzda.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2papvxypk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ernfdhir.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vlpbuqfu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2lkrqndej.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2oxrkfklw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zpvvcwpb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2lxnqkmij.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2xikabhky.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2swuogofd.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2qozychpo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ktpwjmpa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2iurzaxsu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2dprkcltb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dxoxuhzt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2znrpnfcf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2hnzqxctr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2aaiqfcjf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hmloltgx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2nisaldfb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vrejbrxk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2fyivhfqf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qitndyxt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ookbqqkz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2vhqsmdea.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2cjdaeqvg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2zvkgking.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2yivjwbta.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2retjncqh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2eeonkrrn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2hpdkdkvr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2amepxfub.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2nlzdzegv.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vcrnvtfv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2muczxhem.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2agniegje.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hbuypegp.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2mwwwadxa.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2zkbkhqbw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2hqnqpqxd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2pgjbihoq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2omnsokhx.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2xlamrmxp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2kqdazxzl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2htdmpwgh.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2wqxmwzxu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2uidadsdq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2offohsai.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2fuvqdtoz.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2rlqvfalg.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qparbcjj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2mspmnpij.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2btezlntn.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2isdkkhtk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2wodqzpag.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ssdnqegi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2zugwmlxw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2duouhehz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2atiallsa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2olbfzjxi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2btiwhkmi.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2tzfdieap.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ccqhfqmg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2phbqetcl.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2svoimyku.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2tvzmnasq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kvolskru.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qbgdthan.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebthvywd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nsmffdfa.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2igowmlkw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2whvbpmsl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2vctwxfdr.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2bxyuuryo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2cdbmfrgt.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2uraabagw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvtomfoy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2dlqoynxo.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2myxtvkyg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ylpblded.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2hqftbwji.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2dtgbzwde.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2delfqtws.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2pnqaorth.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2sqcqqyyh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2zeexnxtw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2oqubmczl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ufsatwwb.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2cbkepcbk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ndlykkve.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ylhkiaiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ttssgizo.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2epwweucy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xruxgoyu.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2brlmnjaj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2bjvthgyk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2veckvzmt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jqtezqov.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2wvyitaep.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2inslnegq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2zifdxdlq.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2omskrxow.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2fihrmbyh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2yarczhok.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2pypwbcfz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2byuxlwxj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2rqafsnuy.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cwajanpv.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2lvkkukfj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sjwvornh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2xbjxknye.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2lmkyrvvz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2xajaklrg.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2fdeblnmd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2rehuwlty.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2vqyrmtdi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2brwngzzu.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vhxngbwf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2oasbgzyb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2jnzlwetm.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xqvrfjht.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2cbducyya.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2dpfxibet.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nbgvnrmd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2okiurdzf.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wnolkjnr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uklvpqoq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2fltwkdol.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2xkywugfz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2xhjfisrx.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2mpyuxatg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fddhploj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bhmvrjkz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2cncjkiot.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2gdkkpuiw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2guocfydx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ivvtxvxz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rfbnrmkh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mxraryhk.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zzrluryj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ukbnamof.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ebbloald.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2pqftdwzj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tcrtxnoh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2evyypcrg.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mvzrfzfc.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2uzjsyqyw.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2qnhpmobi.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2wlglrdgj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2xsfsybcd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pzielyfj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dwwztczb.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2veqtwwsr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ktinzvmg.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2cmyecxfc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2dixpdiff.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dewudqer.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2sabrliis.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wnrsjmoz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ydljidti.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2awhhdlyx.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2lvlnzabt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uvdzmkgi.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2yabhirgw.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zwhiklph.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rshaghgp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2kihcuxbe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kypoioeq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2iounvvvi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2zygpeapy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ognsadiy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2vdgonocf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ogkporrh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2wgovebwz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ytwfuwwz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2jerlclkl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2biakhfmt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xonqikcu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2kecejvag.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2bbuzgiae.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2oaezvfpi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2zwicqbyu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2remlpkan.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2pggkshxd.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2mwzclphk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2zhmoznxq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2rlnkezkv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2msmgibgh.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2iasakvxt.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xttquvna.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2rhxfrswa.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ieunydce.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2qwdumujd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2mhgzmmba.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2zfwsznuy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2jnmvzwip.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wuhydypu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xlazcmve.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2fjavgtba.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qeopfbnd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ppbazgnw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2dwkofdht.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2qwyamlfu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pwcrihyl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jhieogdp.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oopjljtk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gratpmfi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2pacbxwog.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2qibgecgx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2bqvoexvv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zkdutltl.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2bjwuuiqg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2idvpfdbi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jhawpdtn.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aaosabtj.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2faajxfob.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tofzsgkj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2amhygoin.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2glkcgfqj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qvntxdaw.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ajfebmmu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qtwkllnr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yngxyguq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tzbycfvj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zennyjbn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2iykbjeys.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qdnvnomd.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ussmseaq.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yjydyodb.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2cqzbbtsg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2svjjczyg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ccgxxvkk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dmfonioi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ooiynzon.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2clenkcbq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2dougbkkq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wbybldrk.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2axjbbjex.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2wdnypkex.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gdhamkgf.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lzeghdss.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2fvxnmpng.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2mjgqmvbt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kbwefaqf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2iijmicsl.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2nsprytwy.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ujjpochp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2bacuajik.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2utvsuvte.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2gcjvayjf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2pcrqrrds.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2rufssvcm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2irpzmgpn.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2lzumknwo.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2vlblyhjr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uabfmicg.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2nrrofzre.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2asdvnbjc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2usgdjhah.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2pmowbalr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2cszznrgk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ewfrdfrg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2cjnfxoxq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2pusjozox.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2uysslzsh.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mipemjen.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2thlmkyav.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nnplgweq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2lmryrhex.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xsxjhemc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2swmohuna.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2jeaadgfq.html


<!-- 参考信息 -->