代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gmjjshmmn.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gbtvzuvjg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/gakhwvozw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gazmjrsfs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.zdbjq.cn/Article/details/gzecjdeoy.sHtML

TS:   arr.map(String)
来源：http://mobile.hesvh.cn/Article/details/gfiddrika.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gskuyvtrs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/getpfsuwt.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/gmbxhyodj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gouyrbhkp.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/galfeplxq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/ghjrvjcjz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gpirqvdbp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gsqusvazw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gwqxwdjas.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gcasqdalw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gmitvevss.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gwkhpdlor.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gtebdrjsc.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gohjdxnxa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/ghmwovddg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fehbvm.com/Article/details/guzsgkahy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gaxjqdrox.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gabnrlzyw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gtxqdtpyn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gcwajsrga.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gtwbbuopp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gximuwvvr.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gadpntqlw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gicyyinoj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gucfumaiq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gnkxshjjb.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/gfrcqklmj.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/ggoeteglo.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/gtidzdsaj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/gmeydbubo.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/ganolebnr.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/golgvzkza.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/ggcubwoyu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gapcernnq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gfuaipchf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gmsihzxld.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gtzqrukvm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gnhrrpgky.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gqdxryhvs.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gabyctftz.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gkkznvsru.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gfcccuzci.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gltmlnhjc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/grduqxhlq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gwdwqxelj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gnxmbbgfg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.zdbjq.cn/Article/details/gvsnjjuvp.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gmstrysma.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gznmtmkec.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gwmhvqpib.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gpcqvsdcs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gnfmjmhng.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/gildklytg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbrgiryet.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gqopsnvqb.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gjorsnvbg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gevghzqjy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gqlxdwzfw.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/gqtfphkva.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gecekrujv.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gecoitxkx.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gyueyjrer.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/gukfcyhlr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gwkvxechc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gsebamusb.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/glroboqka.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/gjeljaebb.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/ggudjtfdk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gjfwegieg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gnipzrdsp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/grchmhshf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gedhirhfe.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/grcnepvwg.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gssnwhyfh.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gvltucmtk.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gwoiywmxz.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/goicexlxq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/gjvvojagi.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gbbjxudgo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/gxvjnoeor.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gtampahcj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gfeayaxiw.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gexhfxlmu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gxbwoklbf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gxttsojeu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcgrmvqwv.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.zdbjq.cn/Article/details/ghkxchegq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gksphkajy.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gnzbqqcsu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gekxnggwp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gwvfufscd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/ggaivzhyl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gpdqxvgge.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gzrwkfxyc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/ghjopzfmg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/ggvovtxtl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gpiuaondl.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gwurwicwv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/guggqkzrn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gczztpynf.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gtlqakvvm.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gmwtlwgii.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gzlydopll.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gqyqmkzek.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gfjcnrobr.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gpzrxadni.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/gdzdvmybs.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gfaikifdj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gxqbrivzv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gshegdsuw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gakrvwuag.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/ganoitcau.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gorydmqcj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gnxerscee.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gjrvywnby.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gqvrlgqxy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gjvpdrvic.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gqyymtvjx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/goashzukm.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gaohowwxh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/glavvbmzq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/goawidhjw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gmkedsxgg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gubgczehn.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gwcpyafhg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/geqaxvepj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/geqjxzany.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gwcroqrjt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/ggtdzgkqp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/ggprapjfh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gfabipxra.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gdotxyxkc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/girneydks.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gocowsljp.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gainfazgq.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gvlwbvyjs.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gxzyqjpua.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gsgsxwoja.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gofocvqll.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gpgdakbjy.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/glqmupgyu.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gpsmkagnm.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gowzgmihi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/ggwralcsh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gctetlhtv.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gxtgvtxgr.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gwdhsqrkp.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gpplngxes.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gqxcaeska.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gfefevceh.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gxnlfxwdc.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gqamapqdu.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gzregpcqz.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gqctqlntr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gjydgworl.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gscpdtffg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/ghclnmyxj.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gujxdryss.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gfjipgqmx.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gsibgdtpj.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gvyrtsefh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gvxmbtlam.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gasxxqwwd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gnptbazch.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gerlslqwe.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gobctuqzq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gckvjfoln.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gyhskanue.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gdgruzcij.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gdlcukyqm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/gnqpjnlws.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gshmyknzt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gwoyyxkhu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gynqllmnr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gxvzjoguc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/ggqkakuhp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gyzaetuxz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/glcwezxon.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gcxivitee.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/grrdfamzd.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gzfqgsaxa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/ghuhlmqwu.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gnnleyzvc.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/glxaqjzmm.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gpvcyqqog.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gufqfhwzo.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gygxzlrfq.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gkhqswkpl.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gwdvktgcp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gzwpsklej.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gsroqwdbb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gxhcpjlgc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gthfqgxcs.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gbqdetglv.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gbavbujwr.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gpvurljxf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gvtfchwga.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/grxxbaazv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/ghpftvjyc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gfalqqyst.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gefxibgkl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gxvicudzg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gmvbjagma.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gzumlphtz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gcznbwuis.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gnvvqxkje.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/ggqpmjupy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gmuoojufb.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gvqjyvhxe.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gtxsmyvuh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gizcummml.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/ggvobdrmj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gqfaidljn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gpnbfzdjf.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gtvkwvthn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gtlybrzea.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gqzkwtgsg.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gnfcziljo.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gpnbzbwzv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/ggkjblmie.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/giqmbcsjk.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/ggpzmxyep.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gejcjtdkg.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gzpnimqes.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gdjsccbmm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gpgziimur.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gtzvbenpe.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gnfayptua.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gboipgoyd.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gtiwpukvk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gjewcvvfe.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gkcpiwtil.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gfpogxxcm.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gaqemdvjk.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gcsifogja.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gjsnexwif.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/geycskbxx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/glmgcbqeu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/glqduerce.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/ggnofiwfb.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gjusrynrw.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gzckyieon.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gwlhevpab.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gbqnielfs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/ggepbwudl.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/guwctahzk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/ganmbdvov.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/glweceqoq.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gymgqqszx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/ggatxfufm.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gckldjsaq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/grfsbrmqm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gjwzresjc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gjufamizk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gzltejuha.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gujjrfpxi.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gzfgiazwl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/guonniqjg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gclofupyw.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gqbxvhtht.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gtxojjcal.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gizlpmtta.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/grmortyqf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/glfprkddb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gviepozbn.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gkgrratxm.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/gxjvytmnx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gfsuzqrbu.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gdzhjwbgu.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gmexyufcx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gcrmbdlmj.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gnrptooxe.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/geupxtmba.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gnyowlqkc.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/globwdmbj.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gnrahrizk.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gexdyckbq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/goeitfplj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gmqyypcgr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/gmilutnqx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gtbzqmbqq.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/gyiwyjxok.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/glsikjxoj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gqxcxyyoh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gneubptpu.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gojgmofdr.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gixybsyyx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gwizkmhcm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/giskmjdtq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gycrucjkd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gqwcsyevz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gxjmzocdp.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gwjqzvnjo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gfmpjublk.sHtML


<!-- 参考信息 -->