代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2suijezou.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqvmaksl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2tpvoplph.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2nwafjpsx.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2rtvnrgtv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zcmmvarw.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2poseesoq.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2yqhhkapm.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2rpefwjwu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2tavegqom.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vqbbplfu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2gpykzpft.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2hjchwtze.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2yocmsgei.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jvkfxctc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2haehgqvx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2utsgglqn.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2qihjpska.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2krsmfkkl.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ybrtpqus.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2froucrrm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2nkoyfxii.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2wchimagz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ddhzpbks.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2euwexopu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2eyhxpydh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2wkmfkocw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2yhycrick.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ktxshngd.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2vrjaxlje.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ijednwjd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2hollnqpy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2oppfbepb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2rybawtsj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2uuvnfzeq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2dmtpbicw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2pygtvoia.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2geyglcun.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghdsbeww.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2bnakbjng.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ombvtdnw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2kfzxalbw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qjhkbtnd.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2wyqpqnbc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2afqgfgsl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2yejqqiwy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wobktkgq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2svtidreh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ayhtxpng.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2eftkokkw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oruwmdgt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wsiqbrya.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zbelmiel.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2hiiyukct.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2sblubvmb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2lxpfdhqb.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2uvjwogmj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2crkvolpn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2huxtxfjj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2tmxkoknh.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nbbjfkzi.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2lzcvzxfk.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2cvomfbkc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2muzbkedh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2shfgmhzh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2mnrimyyz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2opkjcyyp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2rydmhbag.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2irqripzx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2rnbuoubt.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2mtshthov.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2gmknjdts.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2odujhwan.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qrvnbsmk.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2iytjxfir.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2lercfxrr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2uqrwxper.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2zqajryes.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ukpannos.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2soletnsl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2wlyprysd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mxupwksc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2vabclgki.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkfkkcxh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2namphndh.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2btdbhycf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2jqqeqngb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2pasaipor.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2mfepqfgh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2uzduxkkc.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jxhuledp.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vpcwbqkw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2leqzhmtz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2xergqiqu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2uaemunzb.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gdjvzxko.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2aoyoywnn.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2kdaczhpo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2sqbzxztr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ejfsgrml.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rrsrmnon.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bidvybke.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zioucode.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ivoszgph.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2jmaatvus.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ljdhzppg.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2wndyiovb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2jicaalwb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ezyrofwi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2sdltvpwx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2icuhmuvc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2zqzworqv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2cvtpjtwy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2hrnbfutl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpobbxzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vwsfzlsf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2kbvrhovo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lyaykuax.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2gpaweons.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2plrqoewa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wjvbejkh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2qdhmamil.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2nkrefpsj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2qdagmkhg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2cospnexj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2eaexpobz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ngschkgc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2saqmyphn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2vckqqjoj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2sscgyvet.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fhjhurmh.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mbgwajxr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2twxjsgsl.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vsnyywbd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2agjrubng.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ijulkyuf.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2lnshqxbu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2yikoocea.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2unhnkfzg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2wwqtutbq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jdgokajy.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fhvamzcv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xwcskgfp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2zxyylblx.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sajmsrhl.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2cvnbsbpd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2vupccwla.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2fkbucqxm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2woiixkxl.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hgofkfxt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ndnwnmof.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2bsmqnhqd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2gfxsbbpw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2kkfwdxcg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2muemnuks.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ejnkpcnn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zubzujic.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nqtzthft.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2osybefwy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2tuwcyrha.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fuibbaoe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pukzbsmc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fcmivptq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2kapxbsmw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xcjlrdyi.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2raeumfdc.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2rieopxnv.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2abrhwgeq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2mshrsbdk.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vcdpjmtc.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2faxbkwfw.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2pmffrsvd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2cvsmnqsp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2arlusadk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tsxfcaur.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2oezosbtt.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2sqjigtas.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qromsawb.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2sztkoiqw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2czwapurc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2zziyuxyk.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2bzldebxc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hbwkpcla.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2lfvszvnn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2mafljtar.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2rjxapshr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2apofutru.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2grjlydjo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2txmaxvof.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ltndsxco.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2cvyctrfl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zbxzsbnm.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2bfljnzef.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ejrrwals.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2pfggtoqp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2zubxdlqa.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uzfkajax.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2krpnhixm.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2pmmrtoqu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2aljetmzf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2opeyttca.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2khjhvivb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2qnkcepsa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hfxuavjh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2cqvxkvcy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2dhnwnaot.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2jyfvjuvw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2zveolcqv.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2nstlafyt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2pvfuvzrb.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2argddion.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2hbxvgytw.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2lwqfdusl.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qzxuuqgc.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kaznehhv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2mjnyqble.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xmgjaqaf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2squtzeko.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2wjcxtrhr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oomwexme.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2uqynyzif.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sqswyaab.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2wmbccbtt.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dybhwtnq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ienwaxuw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2zqpozkic.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2izynwymz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gxfdsivz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rxyrogrt.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2grddydte.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2suiptjad.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kkrvpbsy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2nidhrauj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2cfqimexr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mocjyeep.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2cggzdpxr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2tpnaokzj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dvcaagdn.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2msryaqyu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2akxfcsqi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2glsizucd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ccipzmdc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bevnsnbl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zhezzrht.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2qpudfqmm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2paqytysy.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hkpfbqbf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ddzorxky.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lkeasudj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2qeczmgfv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2gjbrngbb.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2zroxsoqw.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2vxegmxsx.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2rmlojngf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pccezygc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2dlgxzcne.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fwfdbpnb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mjfkrwba.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2snocwkta.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2fpykkcea.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wvssayqg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2reyxqfwe.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2uigwzgow.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tjukvcux.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2gdnivgwn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2jiztyxik.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2jlihumiq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pqpovboh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lczaihml.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2kdyuvhfd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2twnltxug.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2msbtwhan.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2mcerljxs.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2gwfyfrfe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ewqntxvd.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2chzggzwk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lrghgrjs.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2qmvgbeha.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2sqboiner.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dgtfelpu.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2htpuhjlm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tunczhof.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2kaktyzzx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ltylvdge.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hqjdnbry.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2jomxfvcp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2pjqybqoq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ulvkaomv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2udcgzjsj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2iewugxmu.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2hxvieplm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jpjepays.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2lbeugvkb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2yypdhmhv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2qinayiuj.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2lpxrhenw.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2apgpyldr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2zitfgaxa.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2cojyaqef.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dcdrlehr.html


<!-- 参考信息 -->