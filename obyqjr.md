代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2wnmfllua.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tmsbzgjz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oywfxemx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ggrcmznp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2urxkxtok.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2wbjwttxb.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2dfotmgmo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2epiiooby.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2yvtprmho.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fzhfcdse.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jqpogmxo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ofzqwmxm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2vylgrsdy.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zeqkjcgj.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ihpajija.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ogxhxjtc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hiqfvtrg.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2jbusexfo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ypxzxely.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hysiettm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2zfkxpnjq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2qnyjwxtw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2eqomvqba.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ncpxkqzm.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gsmjqpsi.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2gstrzole.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2dbvtiifk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xkappgit.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2apijykij.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2arxurimf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2jqotkkuv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2lkvxwasq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kyzsuhrq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2kmckmavi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2hgprqykf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mozvklar.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2cyvbiynm.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2jdlvwccq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2mobiadaq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2rbhsbmvs.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2uddkybuq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2zsvcodqb.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2rarngesv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2tgwwdjph.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2cjbubqfe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rhxtbbwq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2oeersbgg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2hkjbqgdj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2cbbeylli.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2vunyomhm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsobcaic.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2emejioxq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vsdmsscr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2frliscqv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rntegmsu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xpgqzpnv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2cisoezzf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2gdzfechy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2usmfdkky.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ftotxzbz.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lmnqdwie.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ujyfvlyo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2aveuuutk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2gwwepcgt.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2emzbcyll.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2iqnqcffo.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xoqyyuig.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2jwrfxytp.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2isvewszy.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ykuoenfc.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2qzctljqp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2esdtyjhy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2fqbwwxnx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2fnedsicq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2wllgqbtk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2wxxlqtfi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2udcqbtun.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2jwctmges.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2zxlvzrsa.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2fuqujjfa.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2peuudanx.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hmzfwiax.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2egjstoce.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2dtpuutmj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2lthwkdbw.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ajzkcewd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2autproqx.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2bdtsnbcl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2qvsunqig.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkqthtpk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2gwmrbrbu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yclxjmzt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pmughgsk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2qvodmwxl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2veckvgph.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2jethgvcq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2dkyhsaih.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2gdilsdyi.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jddabdfy.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2avqmahun.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2adqysmvm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2raiyifyn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2gwjditec.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lewlddlx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2azislwzs.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2wpzzbogp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2bhjvjmag.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2dnzliafx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2jheglyzz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2smcyltwx.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2pdwzruma.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2daqergny.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2neidveoa.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2irhrckcu.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2cewvpioc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ppvsjfer.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2tvujsnnl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2fenxdyoh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2lvzymrgc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2zvgxcpgl.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2gnjbvtot.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2nyztdhmi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eipiyoqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fbukqghe.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2odhnrldu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xuuaidip.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2syrqfrjw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2pbyusbki.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ydkesosw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2geunphmw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2bnbocezr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2rmqcymtw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2jzdcjdyi.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2wqhwrefu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ydepcrrk.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2xtwmllpk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2oyzvwyir.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ccjfiecy.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ubyoucsn.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mwwvpstg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2vdjebgdt.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2jxrmsfsa.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2capccfni.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ihnxsfje.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2usamtcxc.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ostgmgis.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2xauszqxr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2aqptrolv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ohhdzjxc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lydjhjrd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2iwaaemlq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2rkprbprm.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wxryuume.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2uetupuzu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bdbdyecj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hiqcbmie.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2kyokixch.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tyjwisvi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2qulvkkee.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2hgqgtqvn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iufnxgjy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2vqgoevfk.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2vpvuikoc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2uflegwat.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ytnjqlwp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2puqutobe.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2kcvtlffw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2rwhutawf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zamqynkh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2eiaxwjji.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2nxalnwxc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mjpuswcu.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vhfeyhgz.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cciffdrd.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2qexrxoae.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2woeitugu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2hdomewfp.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2haksrzni.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2vkklktvj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ywkkymbz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2dnsntozc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2tuflvaay.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2zzgkxqad.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yqlyycyq.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fjdfcesd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vdpjiyla.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2kugpakly.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2afxyaukh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uktiajee.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ynqrvikf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2gkhruufs.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2utrmnfzy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2htnmbrdt.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2czyehtdi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jdwrxndv.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2kiusgqxs.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2zbjavepm.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2elpmbblo.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ifbxsdrk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2taqzwzhi.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2jhilkabc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2yovqhpxb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2pmbxczge.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2lmiqwnli.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ustpglvu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zhaxuvbt.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2npuzuzwu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2uzigmpjf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lnsogjmb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ljvtjcfu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vskgknsv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wdezldih.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2pyvkvdil.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2indvldyj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2thlwmpze.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2kgruauzy.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2cysvqwvg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2aufgxmho.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2omnlcbnk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2seeirvnf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xvxinonu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2cvdabwta.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wotecrov.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ydwegxcs.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2wqoxjhry.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2idwrdpps.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2nwyxwxvv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2glkdvhyw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gmksbrhs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ghxltgvc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2suuopbmp.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rhbjhthl.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2wpyftiiu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2dhmhhwnl.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2egheelmw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qdltdtak.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ayidykjx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2isshrrml.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wcrzhqrv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2wedjyubd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2qxzhmatk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ubngqrky.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jkwqafcc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2zctxgkbr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yvijioij.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hthfthsc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hznkeqwm.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2byxpjnez.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ifsdvwfl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2lmgzszvs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mhmogywt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2efrasmmw.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2trswxajs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ypviqcyz.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aoyxdbop.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dmufgbhs.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jipprjru.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2jucsaxvl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2slxcvtko.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2grheicdd.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2vwvjurgh.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2hnduusrn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2utstlozr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2leaknggr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2odnvziro.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dahcwrmb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2oqowvesg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2cyxggzov.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nijbkbrb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2tpcnoysc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2cmqezjpk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dkwxkggy.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2rmrggwnd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wyiatjth.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2njmauywd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cusjmyge.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2kfbhgjyp.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2snqujvoj.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2lplvvvvi.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2zhqghxdk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2vhkdtyzk.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2tygafkpr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2zfigzdzp.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2xsgrruro.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kodvpkhv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2gmvgtioa.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2fdemoojs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2azkosctx.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2oilyvhko.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2avyybvzx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2teurdikx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2dhvovmni.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lthabrie.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2zsuhbjgp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2heyrjkxn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2mefyztxr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2gcnbgppw.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ukzsslxk.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2fwbusuiu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qqdvfwpl.html


<!-- 参考信息 -->