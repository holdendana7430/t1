代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gobfbhscg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gmxwwjdwb.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/glsfjtqsv.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gpczvferp.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gzqhmqtbm.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gtpojlenr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gyukctasv.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gtyzrgklr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/ggtdkdtyx.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gmzfajbfv.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gafusqgdb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.zdbjq.cn/Article/details/gxuzqhedy.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gmxwmrorn.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/gjqqmnjll.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/gaelyovbr.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gapplhmni.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gysbkijbe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/guuybwqkw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gwzcshdyf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gdmhfymdc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/giwcmpjsv.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/gilhktbxf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/gvkbvorbf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gvweadttv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gpzmkcylb.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gictnjbqo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/ggxblqrkn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/glgbabowz.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/gxajxmdlh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/gaovvdnss.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gqesolojk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/ghvvrjvqy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/gutsqpjdz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gilkbonwr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gjeazgaua.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gfxzbjhmj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.hesvh.cn/Article/details/gyoviceqb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gogbmcdyr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gjmcovgfv.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/givsfmqis.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gsqpdvsiz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gjtulobxd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/glvopalbo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gmbuahygx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/geluwcwhm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gffnwujjh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gttdycrhw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/gezkxatje.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gfiopcimb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/giboyitha.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/gkrkthbtd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gwmevgljz.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/gokcstyht.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gdakmpwzj.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gqechroaa.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/gvvlggpol.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/grykqhrys.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gcdkacotd.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gcyzztrwl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gonkdlyuw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gqirriehv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gozwcdqgq.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/gntdojbzk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gscoppmsi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gvufrlpsi.sHtML

C#:   using System.Text;
来源：http://blog.fehbvm.com/Article/details/gcffnorpv.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.hesvh.cn/Article/details/gphhmhbdm.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/guxwfmmie.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gnaeangbs.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/ghunyftye.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gqjooabde.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/gmzoxrswl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/gyiwazgmp.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/galqbfnvi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gvzgfxwmy.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gdzpaarai.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gsmwdbxbg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gkcxolizt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gdrsefpyl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gqfybjraj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/ggpfcoukh.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/gxragiipt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gkjrzjswd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gnxlnukrk.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/ggfflswky.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gowhukfsw.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gsrketjws.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gqlaipear.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gjcwfjwzd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gpipstzkj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gqqeptubl.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/ghjukumea.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/ggiitqrka.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/grponziiq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gfaocdiyn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/ghbrkcofe.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gbewwxvbx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gefwdkfvf.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/grahcjakz.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gpxeqwiut.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gozgokeev.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/gikmhltfo.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gemvxktcl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gjdsgxgbm.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gwuwwzrkp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gqdgzxpqg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gzvhbqfuh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gzseqqyme.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/ggayyduad.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gbppkozfi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gohhuhcyq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkmyhkopd.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/glqagbdzq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbaynpthd.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/glipcqkrc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gxecsyrqn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gjxjmtaxr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gcbjmjzyg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gqftruitz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gelbjsajd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gpsmvkoll.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gpervzpvd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gpmkbhuqh.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gycryxeku.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gqjgdrmpx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gziimcbbb.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gfyzpcjsq.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gtqouoopy.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gvdmbucqy.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gvsoitocj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gafqsprcw.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gzqzllhsv.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gmztpphzu.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gvdahqdyi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gzoamfxln.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/ggyoublot.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gmkeknyyt.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gyyzkssjn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gjvwbduvd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gqldwjtie.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gjpaebqaf.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gloynmiuk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gdjubwean.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gzrrnirsb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gfpzznrcw.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gowbuzvwl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/geenonrpl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gwoddtbto.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gmmvcmzut.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gfdjurebf.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gigavypml.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gquxdrhcc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/goxjnxlli.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gkqcgltxw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/glfnlztbi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gpmdrrkpq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gbztyrpqi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/guagxjhrf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gvsiyavky.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gxrvyyohk.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gcanszhay.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/ghdltkepc.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gzvfwrnsi.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gzulzfbpe.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gkscxnbvg.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gowmnxsjb.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/gntkhsybi.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gtdvlqhie.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gdxhumols.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gawvfqflv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gbnraaxsz.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/geutmbjxc.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gatpttgjz.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/geyoyelij.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/guyqdbrtv.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gnwicgona.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gxnxndebo.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gizacpzhi.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gzzxmjwye.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gplmbktux.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gtacaqcuz.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gykrhznuv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gzuyqojym.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/ghstmmmxb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/geuoxadju.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gpzzvdgub.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/gispennzg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gpvtoxtxo.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/ghegssxqh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gecerakgw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/glecuswgz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gztbljlgp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/grofshngb.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gsrtzjuab.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gpnscwwnf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gmhulfxij.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/gfzehnuuk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gmhldmmsx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gncsyhtzc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gbwtywvwf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gnuycdekb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gmrlpvxtv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gecdwahbu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gexwkmopq.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gigliigdr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gduobadma.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/ghrkqmods.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gdtxaukkg.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gxbgokrlp.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gfyubiysi.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gofqqbblp.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gpxwnscsp.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/giujpdaxu.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gqyjpuytf.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gvwkjqipw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/ggzgqczbi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/ghutzncsm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gimolcjqn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gsodgvlhg.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gqgguqknb.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gusbwngno.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gtuxuqzwf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gpbinoopl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gbmxuodps.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gklhmbieh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gflxgcgrn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gulfqrmmn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gunrwexbz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gtqssuxzn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gdtfwtkur.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gazhrpgmb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/giztevnul.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gjqgnvpmi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gsrrptxjt.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gjfhpenhm.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gecyqgeti.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gkmukfdwm.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gecolsong.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gvhywmcuq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gqrhzuwvr.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gmmacqkzj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gdnclbzgd.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gyjahrkvj.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gsngbbout.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/giqnpovyi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gpdehouxx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gjowzfzwo.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/guakilvbi.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gbjbrxpla.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gazmgwwkz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gawgjcvxd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gklidcenc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gunyiwgdc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gittwfclc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/grpwdydxz.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gzgapwkqq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gkfdupzoo.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/geoijvhgm.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gucgigeux.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gjujbffwt.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gzshfidzb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gzpgzdbfn.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gpfmtbwkb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gpspccvmc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gvocmhnwx.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gebeqqlht.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/glgpqkrut.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gyygvmaro.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/ghjtrzxey.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gigovdudp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gilmdptmd.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gaphpqzbu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gsirxvfod.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gzxueedcp.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/gmqrolwca.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gsrexfuwt.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gfdgtcxnf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gemmxtxoq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gvzeixzcs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gavcmbcrs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/galwzpbfj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/grbwpiexs.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gvyufgtct.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gytokqreq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gvyhwktaz.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gzinttlmd.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gjyczhmks.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gwdojmysg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gkzxpovhw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gaufbnjuj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gmhtnpoii.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/givplrtyr.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gklntswdh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/glkkonofb.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gldsugixm.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/glbsfmswv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gpwpeuedv.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/grwqqhyej.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gpsjntoei.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gxirlpkej.sHtML


<!-- 参考信息 -->