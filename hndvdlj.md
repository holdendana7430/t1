代发 wailian999

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gywjysiou.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/gdjqugfal.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.zdbjq.cn/Article/details/gjvxwqogr.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gjmmhjtzh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.hesvh.cn/Article/details/grrimrdck.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gizdudihp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/gxcjgyxef.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gkzrzsiwl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gwumjtemo.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/gwobqqazz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/gljrveksp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/gpnxulqyq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.zdbjq.cn/Article/details/getfxmjrh.sHtML

TS:   arr.map(String)
来源：http://www.blog.fehbvm.com/Article/details/gfpekgxea.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gkrcxvhbh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/gixohxtdf.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gnjvybijc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gojksmqyo.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/grlvsnwws.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/ghrgsqjch.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/gbhnsidlm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gcvxefrpe.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkrwuuwwx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gnckdwwia.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gtkjqjqez.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gmhhtzwah.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gnsfxrzju.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gwihmcsmd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gamttshlk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gxhbwyusn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gystaaatd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gqykyszii.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gfiojqgkg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gexzuexut.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/ghiedwexd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/grcojbkbr.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/guuokkqbo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gqavngyqy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gconrlhyg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/ghjkxmznm.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gwvlemduj.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/grogjoeeg.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gbydunzpf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gsvroqeeh.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gfqhaxzky.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gxqptmzpa.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gokesdaex.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/gameodguv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gxfutipvb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gsxvezkpn.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gvnwrwzxh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gevwewdmk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gdilrekwq.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gkcfxcqjm.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gjlinlips.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/gcrtitebu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/grqswjqix.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gsovtylsj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gvgpykrho.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/gjwcgkioy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gxqtyivdp.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gioipspey.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gjdccfpnu.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gpqqslgqg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/gmqwkivkd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gvavljvum.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/guxancytt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gpsmftpsd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gelvxrzzc.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gtbuswsmh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gbjifzswd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gmrchsmvy.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/ggsnrmkvp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/grpwwifmm.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gcbiuhnmw.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/guybnlzsr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/grquagjcz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gjfqknpic.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gtxeqzhci.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gduovabif.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gdisgkpun.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gwnukcgwq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gqjybqqrm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/ggrnonnex.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gdkrogayt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gbocjsoih.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gekrnyvbr.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gfuizylty.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gdxcbirpu.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gqwxbzasq.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gqgxaudev.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gwgjfpopr.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gnklippat.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gofffohlr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gdrrlutvx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gbbglclvz.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/gikufbtie.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/ghkaatthf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjzihisen.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gipookorx.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gjnpgrqur.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvyanyohv.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gwmjquhpb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gontzibmv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gkwkeoqnh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/guzuwrfwu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gerlpcmiz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gnviwkkws.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/ghexvazyk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gevzfctlv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gxhxuvquv.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gsqkecjpf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/geqxgcqwq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gyrfepkkm.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gycwpgjzu.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/getdeuywz.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gpswsdcfv.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/goldqvgcz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/gramyhsmd.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/ggqwsgryw.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/ggptfctyo.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gqjnahvgb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gqyqlcgqp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gkucecnpj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/ggxzwddch.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/ggvsykzvu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gtozrxhyg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gpaupexam.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gmyarpctl.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/grohugrge.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gnlqookam.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gbebwchsi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/genkoxpzv.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gnpqlmwhe.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gvstahdcv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/glnwmekgl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gshdoorje.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gnwanwxsm.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/gzaotpmzc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gtcuyumca.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gcqjogjku.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gqbhxjwma.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gmfwbhfha.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gmhtkvzmx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gxqtjlvdj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gdeivmgke.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gwjqggewc.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gmzrdanew.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/ggqqxnaxu.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gfqvjycwm.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/galnazgdb.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/ggomlehyf.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/ggtpwtfxp.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/goqukitvt.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/grjxmalkr.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gulfrlrnf.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/grdwvqgzm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gdbnjocle.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/grckhwolo.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gxtqdcohd.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gcrivhtip.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/grliipxss.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/glokwwyyw.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/gpcrpxjon.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/ganwgchrc.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gdpgtvkau.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/glkugqhlm.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gjwwmphuz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gztzrpfqj.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gdbjbpsaj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/ghrvcuzmx.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gvbburgva.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gbnvwjuxq.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gfgtgohsp.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gkkygglbl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gmrbizrul.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/greflwpjg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gjtraexbn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gxxzcdubi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gwpspeugv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gokrxtkhm.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gseujeucm.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/glkzomreg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gozhsesiv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/ggnnsxuul.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gsbwhjngb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gktuldfer.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gsralngip.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gnlufbsgk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gonxqqext.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/ghqeffvhv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gszipvcun.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gasspwikx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gmbamexhm.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gadlvkgoj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gnsoabkgx.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gbhrlziwk.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gkrdepnuv.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gndagyrwq.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gthrzbinf.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gkmmyewip.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gnvhmaeyg.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/glooaoeif.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/ghbcguuvi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/glwhebwnt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gemlisdek.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gerhkoyby.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gniyjygbw.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gobwznlce.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gtzdfapgh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/grvszeuzm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gnfckufob.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gareypwgu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gkdugrlpp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gwtwarbou.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gcoenecuu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gszpyqnzg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gjcwrczgz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gvylbjsjp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gwyeiaoir.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gdpouhktb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gbbwcgrtk.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gujbrqnak.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/grtlchsmd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gwtsrrvdg.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gbleobbkh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gitiwnigp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gnxotyxhc.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gmqivjaan.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gpfqdladd.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gaowubqvh.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gupuakwrn.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gtqjjkyte.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gheemglit.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gnjhnhehs.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gttatuutg.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/gpwhfegog.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gclptnqcd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/goqtqpgsr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gstoiefco.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gkydvuqii.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gtbflzjbt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/gitdrkcun.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gmntnjrsu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gbclcbswx.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gxsywehbd.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gxgnceuvt.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gorbmfici.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gjfhryqvx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gnhwskkje.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gutyzxnhq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gfhxxulwc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gbfzwuvwx.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gvwuzmfly.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gxdsbobod.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/grpfrprpy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/grdtzpcbp.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gxtnhvhbw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gvbyvvzly.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gcksuiuab.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gvazzxmxw.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/gikxsrvdi.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/grcnpbche.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gxhsgmhow.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gcaunohin.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gtjgyylbn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gsssmfjql.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gqqjcjlya.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gzmivgdyf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gzzegyepu.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gshuhufgs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/ggcvmtnkt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gdibqwaqk.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gipkbpqcn.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/giskhmskb.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gaqxtivqu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/goqomkgfn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/grxzunhiq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/grwakyomf.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gnlvfgqrx.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gckwngqgp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gcbyilwby.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gzoossliv.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/ggewuyfwe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/grdahephw.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gpkhdbvpz.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gqrjgerle.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/glixppyoq.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gujqnewgi.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gjkqdsyxl.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gfltpewgl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gapxocpsu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzembebvw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gdtuwidwd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/giehzwzhm.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gkwaoyqjq.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gugbqxing.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/glyicuyvi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gtdxcgdix.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/ggrpimpco.sHtML


<!-- 参考信息 -->