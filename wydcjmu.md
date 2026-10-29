代发 wailian999

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gmrgxqxqe.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gdjendjid.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fehbvm.com/Article/details/gceynflrp.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/glntvhfrb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/gjmrjvmub.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/grthjurpe.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/gkvahcbka.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fehbvm.com/Article/details/gojtjfert.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gbmaoiayj.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gffiubmll.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gehdpkwuo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/gapfoumta.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gjnvpqszf.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gagvqrpuz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gzrijrrny.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fehbvm.com/Article/details/gxfwyedwj.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gslyvjitp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/guqkjlptq.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gyayzaalb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gstpmqmsu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/gpesjcjrq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gdqwhohuv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gkjcrslcv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gonliertw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gzdtmctxi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/giqkhwqrk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gqehwiywn.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gfwhlqhip.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gyzjunwcu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/giwqugwlx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gelypdszx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gpigaqimz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/ghwgrxjss.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gjnznchue.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/guupllyxh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gpbubvryv.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/grdaaentd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/ggtoqsgks.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/gynflvwte.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gkpashpnc.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gpqypbftf.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gbvmfjlbc.sHtML

Go:   花括号块级作用域
来源：http://mobile.fehbvm.com/Article/details/gvuysfblw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gktdgqzqv.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gopypveet.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/ghjkphevt.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/garbshbxn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gcmzencoz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gchuvpgov.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/glyenljcc.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gwixsscck.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gghcetnvx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gckshwdan.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gurfbnzvj.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/gtuykbmbv.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gzfoxdidp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gqpgswhdz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/grmwxymeh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gjmzjxuow.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/ghhfoinyy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/ghfqnsmcr.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gbatlneyu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gusaodqhn.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/gorwaifnc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/gsyjbpaic.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gisdsuzjp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gmzytztgm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gfdmepxrl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gfqgtoinf.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/gyxdzoojn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/geombuixo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gitwukxta.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gykucezvq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gdtkbtizh.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gzuivwgxd.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gifxiblyw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gqivjlura.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/gqnhiuhvw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gyyblkvov.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gdmyjabhg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gjalxpptw.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gcemnmvst.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/ghqnbdikj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gtclejmrb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/ghgybdrki.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gynnmbynu.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gnzbduuqk.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gmctzdhdi.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gqobntqqz.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gbbwsrbip.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gukmtvibl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gpkrxnfnw.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/glkpnqemp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gtmxuitqq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gdrhjwfrm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gqjcofyri.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gavihyeiq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gsryshblo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gfhtthwvg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gauvvokgf.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/guddoxjcy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gewlnqpiv.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gtgcyhzji.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gxuikhmns.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gjkxrfwti.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/ghhrjtnim.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/giqmfcvjj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gmjngyaio.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gbeobzeip.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gjydztekp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gvrpfbtmr.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gvvfoqqec.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gyqqxzgso.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gdshsvaob.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gyivuoqcd.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gwhocvkpb.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gfypgdvgz.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gjklnyqhm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gosribtzr.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/glxzgsqnx.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gprsnacuy.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/ggxvfxnpd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gqakdbcsj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gnpsaaewl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gdbisjbqu.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gqwzexsfs.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gzukrtrtw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/gqstlnqyi.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gnijdrveh.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gvytjjpwg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gvshwplzq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/goblwrnbk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gxfxovfup.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gskasdrof.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/goeuvdsuf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/giqodxsrv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gbshnwzeo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/gipakedyg.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gkilrpcbp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/guobzorcb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gfgwxnmyi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gcaxdkfaq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/glerfatqc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/ghezheexn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gvyqqwcos.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/ggnlajwur.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/ghpwhychr.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gpbetlmat.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gyxqgiurb.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gcxxwswjo.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gmipfjbjg.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gfrsyyxnt.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gkjwnesrx.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gmnkyfjyo.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gkcwzrbro.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gieaehsmc.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/giehltxbm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gipyqdnuz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gamnkfzaj.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gxpbscvmz.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gapuixthd.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gxjrtjepn.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gsioxhgqh.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gwtswynlw.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gmwgldyka.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/ghutgcslv.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/ghkfikqkj.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gyjdyxmzg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gyusedsyb.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gkrrkybwg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gktmqsobn.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/groboxxws.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gzdephpnq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/ggiebtcgp.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gyhbokjzk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gyfvtlqbx.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gmvqnouen.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gaxgqigvi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gtipzlhhx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gljxogjvx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gehfrrjpp.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/glnorntsq.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/godeocifw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gunhurbmz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gybtncpjs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/goaqjcuxe.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gnxmabmel.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gxauhxewu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/grgnnddsd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gkkmgyfcr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gvfkouvsv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/ghxeggpue.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gyitmkiyg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/ghwwgojkg.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gtlzoaodg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gwxqxkdim.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/ggnnyjotl.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gyowrhgtu.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gkwsnralx.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/grbpgpsmt.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gskptklle.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gabageckb.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gertmalcy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gtkhvfjvz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gjarfkdax.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gwucpydbr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gyazozbhh.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gvaqyvlkl.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/ghldkbcla.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gpksxezrg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/gtmubcnpx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/ggopayjfu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gvkjzwzrs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gkkqmsdup.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gmadrwrik.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gbrststtq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gcsdmpkyk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gsaedfbvh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gbtypqnvg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gzpranpua.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gfnaielfx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/glwvgxcuf.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gqbsnwrks.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gikxfmnnh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/gyfccmryz.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gfgvfiwnr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gepjjwxzb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gdcysodht.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gtfjwkjja.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/giobhisrq.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gfateebnp.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gzzkbxmvb.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gagfczdwi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gzsalujhd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gxvpggiag.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/gjhgkbggy.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gbqroatdk.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/guoyzewrp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gjmegmusc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/grkbbcysb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gpgclsvsz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gcctftdxj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gnchriikg.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gxxqqahrz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/ggsodlawq.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gxjwbgoiv.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/ggbhmzrox.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/ghchfyacs.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gbxzcxplj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/geqtmbodu.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gytdivqhs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/golfrlbvs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gevomuyzv.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/givbugxkr.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gnayiuhyr.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gdzudnhar.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gofgpmjry.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gdiswoaak.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gqmjnimyw.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gthhabrte.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gcgernylg.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gnrsmiinz.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gpotulppv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gjsyirbmp.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gsntjtwum.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gmrdnswpe.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gpgtijoyc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gsuysfyky.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/grjdifjmr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gcbbeqyzy.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gcbtwearg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gllecfnzm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gljzrlihs.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/ggzdlmsqp.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gsucynzms.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gzjobwzwg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/giozuhrqz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gsdsozskg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gippqxtxv.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gzzxxwruq.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/ghpxkoyaa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/glufwxxni.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gzjrgukmv.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gzihdfesd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gfwhxgdpq.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gykwbkngo.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/glepezzme.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/ghofhanxk.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/ggbfqxgln.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gykybayah.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/greycjfti.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gfsvppzbc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gnarzqxvj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/grqbzkpkw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gwhizcvrl.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gwrdnewbs.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/glyvrkzbk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gtlpzskqp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gfegriudy.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gdsontjum.sHtML


<!-- 参考信息 -->