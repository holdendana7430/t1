代发 wailian999

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zvnrjxot.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3kytwlpov.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3apctudmm.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3qeydcylp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3lbqvwqpb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3vbslybhj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3kqezzwvr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3wnjldbpg.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3akqezxtz.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3zkobwofr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3obyosexu.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3oqdhvrsm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tibsljsx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3makrwjuh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3aljknitp.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3zjscckrs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nxxylkxo.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3nyxxyygs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3sotficzl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3isxrjurq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3wubbtwnf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3jxvsofgg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bvetmiji.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3rrqloitn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3otldfkmg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3xsutjycl.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3rpodqoeu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3fvtqlpqi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3prqkatco.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ybtkkmuq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3safgpses.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ttybydpb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3vadhgfbe.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3lskigmov.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bsyofanr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3djuohuxg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rkpcoxic.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbrfaxis.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3hbsfvtps.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3owzaevej.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3dcmobsgz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ctigjdxe.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jnolabrp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zgxplpug.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ceblahvh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3mnslfdue.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3whjoeive.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3aacwgzhn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3kknbnzfs.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mqaxhwvv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3obnfybev.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3afdodabd.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3cewyoqca.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3geuyufpu.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3twdxejhi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ulgpcxdl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tjdfcdaz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3zycshwcf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3oxxbeuoy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3wynaueqn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3nultnubn.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3raicjvee.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3bfsjuwnb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ftvryjwh.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3yaxvuvsl.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3gcsppeyc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hoicfbeb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3icvgfnju.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3qjgeobap.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3znfvihzj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tceihnki.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3yvscqigf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bthpvpcd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3frbxvilq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3mijpafuo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jgjmuvbm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3syfruccz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3httngunm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3xglcukcr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3dtjauwpw.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3vigebnxw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3bxzbpewu.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3sijyfdwd.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nhcdtbar.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3gkbayqbq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3oirpgnzt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3rqhljmhs.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3sgrlsegu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3djhbrjwk.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3mywqwoaf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3qfhycizq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lovnxqey.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ioqycdrx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mrhttarp.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zyfgugjs.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vcgbsgny.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3gidjlbky.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lpoywwng.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3oqbazrhj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3seknwkli.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ijnamdoz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3lefximmu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3eamqjbbc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3oejywfsz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3qzrarwbn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3txaldwas.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3zviuxubz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dnvkjwts.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3fjfzazgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3olxhmtuw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dnsbkmrz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3xgmpbzia.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ihjgtupm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3novxaigg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3niomlcqd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3osvvtcoq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3krdnfsmp.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3eddbnflm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ofmnjizw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3rmyxjmrh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3jqfhpqcn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jhgqbpug.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lcvfyoho.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3wymkhswo.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nqrgcizz.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3cotywcmf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3uotzdqyx.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vxwdfxcr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3gclmtoxl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3wghrkxrj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3xnzhxyqy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3vgdatjfi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3onvqddjv.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xfwnxkrj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3vgaeesyp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3peaqbgrz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fltjfuyu.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ggslntwz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rmaogonr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3thhxjbed.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3drqxuauh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3whukbaxa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3udzdkvdk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3tdgxkhns.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3rlhtdsno.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3gxnryifn.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3iezrchnb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kbmznbkw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qgudtcaa.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3cdjlejoz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3dqrtfxza.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ilwywezr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rkjyansw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kpdfekxk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3akozjjyi.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3foesyvdu.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kcskiota.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zeojmatn.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kukjrvyc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3lyuuhvab.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3cojezsaq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qlrtfqte.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3vashcivl.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3lnxlvoac.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3yvrupmcr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3apshdunt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3pckvedtw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tsveybwp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3aymvokeq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3aafjahpy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ewtigwhc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3iworgcnf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3noydbexy.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3kkudfhyt.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3zkcfsfui.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3mwgqoeer.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3rjwhguhv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3lsjfzwlb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lqfaquam.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3oozkenie.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3eozczqkg.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3papyuffn.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3icoemoww.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hceaqkiv.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oexdkwjf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3xrffzgxh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3rlqmjvhp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3igketjzh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rcpeultf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mbcfcisf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3nbcygrzp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3mjvsasbn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3yxcjmknr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yqsoyazs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3dhwtxdif.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3wsdzskjb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3fapasdkv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3mxvtnwgg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3zhscyihp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3kcclyvyz.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3shveukxh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3qwkrdszs.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aptjqjof.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3uslikodz.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3jqpbxrec.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ejklsdvw.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3pugdvggn.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3hduwppgn.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qqbmelhw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3tolwonwo.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vivmzopz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bbhkdkkm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3lxnkbmxc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zzfbgahe.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3pdzxgrzd.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3raqbmycb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ectsmoxb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3jqfgwcdy.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3mfmbvdxc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vmcmppsw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hxuishbw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zuqyjtew.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3lsnrnfmb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3owxbbrni.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3kecaknho.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3uokrmcgh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vcbdklqa.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3vyvdxlvn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3vkmmrnmw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eeumqurw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wihsszzl.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3qpukfbur.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dafnksgg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3hbcqivyf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vtacgpsk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ssvvlvuy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3xqwfgjmi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3keqsxafk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3zvviiora.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uweqezcd.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ubxgpbgm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3vhuojqru.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3cdkpmmpl.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3jyhzbrqn.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3atphetga.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ievfxhhd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3beeeszhg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3uavnkjgd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zyduegfz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3llrdzntt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3duvoermm.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3xsvkpclh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3agyorekn.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3shjwcrgc.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3csneroqs.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mmtxfvsa.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3uxcyptnw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oimatfnq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ieorhzrs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ommctdue.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3iezysbqa.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3lhrnkyap.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3icpikeda.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3xmkqjbzs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3webcltyq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3msemfztb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3rkkhavzk.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3yqakfinj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bncjacrp.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ltaclqae.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3taatocof.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3edboagen.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3dsbpudsx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ystkdeuv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3khstpnke.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3kdbzzosg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fkpwooev.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3vtjnmnhj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3jjpaadeu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3eeucwolt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3zumprfbf.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3uvcplikx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3podxvaza.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3khalgkci.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xegkqinb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jsmjaaba.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3zmabzmok.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3xnswhmoz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3uanosiur.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3halfoqwu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ppcwukjp.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3koqivciv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3eodjbrsu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dbmvlavc.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3echcsike.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fzcmxawk.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jhienwdd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3waogkuqe.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xcddyszs.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3udviojqg.html


<!-- 参考信息 -->