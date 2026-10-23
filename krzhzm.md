代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3oohesfgz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3wftiayuk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3kyzpppwz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3czktynwj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3elwhhjyg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xjphptsc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujvdnhbw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3qdsqnzyo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3awggbzcc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3bwthjhoo.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ljruyalu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3etygpkwt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3nikfdael.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3owuhxdre.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3npfeaigk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3nnwxtyin.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3tahmjbrt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ztfcpkef.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vfudalyi.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3gngpysgw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3gjpbrnmb.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ghndzfgv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3iwqyhgei.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3kvqlvnay.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3zyuxdrkp.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qzsidkqb.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3haojffox.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3abrhgnjw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3hbrqswlb.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3jfcyoham.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3txwkpmgf.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qullarze.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vlslsyhe.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3bhplnezp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3cfoumizu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3hiqztlgs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pukhoefr.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3plhomdhi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3smygilin.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kmkreesk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3tydmqbyv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3kkcpjuiy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3koyctkkx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3qaaemzhq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3wwdovxgs.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3uqwiwznk.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tnfhptls.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3qrdpcddm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3fjmfxunq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bnbefexy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcbionwj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3fcqmcgnd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3uiywvnsw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3iriegesf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pvlujyvq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3jjuvhfwf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3gkuufyki.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3xbejeskx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3zmwzlhkh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3atyrugwh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3deioakic.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3fzheuejr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ktbwlnjm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3voscihrm.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qifffbav.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3jtdqffaa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3hfstpdzc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sxvhuixn.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3txczmwgw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3znecyqgt.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ciubilqe.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3khkntyim.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wadysbhu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3mydkrqvx.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3araajrtj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3bxxvrett.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3hprxtcdq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3mqhxxkjv.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3zrxtxmac.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3duqvvvhz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3gdappniv.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3fiycrocp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3skvcsnpq.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ygwzyzdl.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3dbshjdar.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3mnuhsrcg.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3dbdtwhak.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3aokishgu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3bkyaotkx.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3chnqdmnm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kjblxmol.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3vzoqgjeo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3tbfigovm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mpcfjmsn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3imleycgx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbeckoxg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wvpszhyo.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3hkshlfmc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ugyvrnfv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3hsktmilm.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3fehqmwiz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3gsfgoils.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3koqnjssl.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hybfiryr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3uaxipabe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3oanuomti.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3rtclyplf.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uldapkha.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3pfkxmakd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3lmlakutk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3vqsowroi.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3zmaxvmzx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3dwiecikw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ephjtscx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3kagfuprb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3smjjeawg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3smxjngug.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3rnuoqkix.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3mmhrerty.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mmmrjtsd.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3almrhnba.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3aznmfplr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3zvlyoman.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3hpmwvpjs.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3xysjrrda.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3abygeygg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3mneavkkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hwgzsfro.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3mimbkdjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iesrvrnb.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3eilfppqe.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3gxtcwpiv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3eullmtds.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qvvujibu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3nnpmjxma.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3bpwhwuxm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3qfarjwbq.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3cevajxmd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3itfwzwqu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3dezxnouq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3rcmqfluk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3psegmaow.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jrxfknqk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zjvyokfv.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3hpnoxcwo.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vmzelcrt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3tkedtnbk.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dnsumrhx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3yebgrgrg.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iwaqdfdk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3lgduoqgv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3xtvxijdq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ivapxfzs.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wwzirmby.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3rhlkcnmb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3sjjytbio.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hceewosp.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3okreavus.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dkyspolq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3exywllcz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3jwotxvva.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3csxsqwpa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lsmgwrjw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ztmmkuhx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ujjklrwd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3gnfovbgs.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3wencghvd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ddrtrbmi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3svztglsc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3msebodyd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3awbeaylb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3xqgzhrdn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hcmlpfuq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kfyidgfx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vcwawvpz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3kcopjnja.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3foidrych.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qnzajozx.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3uhxngmtu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3hadtekue.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3lkkkcsvr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fuhuooid.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3kdtagagn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3tkteznir.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3mvoiillw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3onrnanfl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qogujgla.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gmkescde.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3uvlranqo.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rnqynzuw.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3xsxzvntz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ljsowqzn.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zyndqkvv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3bzakjytx.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3brrljbev.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ismwbvwy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3yohhtquk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ogrhhexo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dgfronlp.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ubevohrs.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3rliutuhp.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bvvvltej.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3yuyuntya.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3pqnvmhpr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3yphlatti.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3cpkfldsl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3nktuosbv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3efkllcga.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oxdlmwjj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3tcrgbfhq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3sxakjcdb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3rvwzhexv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bgxjqplr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ucozwwsz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3bpbbfpzd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3funxyqmw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3mhwtxdjk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3efzpnvvf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3bprljipm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3awjnbykx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3jozbwbez.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3vlegubsa.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sucukpuc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3merpkkvv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vlvjmwut.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fwtphjpt.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qkvyvjwa.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yunlryyc.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3rsghhcdb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3orekmzpq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3qjhcwufq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vdakfqry.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mmcsobhe.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3oqoqtckj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3dkglbtkn.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3aaeobqcr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dtbjvpri.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3yzwvzjow.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ijmobeoh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3wrpgipir.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hwfprdip.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3psdxuxku.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3bjygfmuh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wgzgqsvr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3eqwiwxuo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3mwdyzqnp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vxhweqye.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3wjdmgfde.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3qspebide.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3feomnfbf.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3pyweglbf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3wuzvfwxj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3mrofpzjf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ixtlnlop.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nfahpziy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gjeuabtg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3hdisurac.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3aprgzgrl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eyrogrfg.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hgnavzlh.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3itnrapgo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3bjdtclgj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3dnotjfyz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3hjlcwgcx.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3niofnpjo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3rqcmoigi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bwxpdxyw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oripcvxv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iwxgjnkd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3mjtyegwu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3srwrgyre.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3qespxjmg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ozdivswk.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3kxmtdcib.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3jlejakei.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qzlhvagi.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3tfkwjeoz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3rkoebrcb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xkvudefm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zsjdqotl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wrpzosjq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3gldgpjuv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3oejgvxad.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3kojvpgxs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3dsbfqmyf.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3hthqenps.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ozcoeiyz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3nbhjsooe.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3zylelqtd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3kmrnrbwl.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ognhjwii.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yglyanuu.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ctmyrhss.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3aqyqipuv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3xjeqjugr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3xpaemtek.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3aijzirxt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3jjdciqmm.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3hvcfxgnl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3bzdyukbq.html


<!-- 参考信息 -->