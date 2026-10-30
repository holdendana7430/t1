代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrtdjies.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdxtyamc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnajuprev.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gevxflrns.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fanxiaobao.xyz/Article/details/goicyslxk.sHtML

TS:   arr.map(String)
来源：http://mobile.fanxiaobao.xyz/Article/details/glondupdb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqgrqxtz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqduovgwx.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwtskzbp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fanxiaobao.xyz/Article/details/gpafekbsa.sHtML

[C08] 闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyylzshns.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fanxiaobao.xyz/Article/details/gcdcvxixk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpuhxxey.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvrjfniwh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghneaddbs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fanxiaobao.xyz/Article/details/gjklnxkqy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fanxiaobao.xyz/Article/details/gythpvrrh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fanxiaobao.xyz/Article/details/gsmesvxpp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goweyqeuw.sHtML

[C09] 递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyaqwofb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjldrmnm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fanxiaobao.xyz/Article/details/goewrgkxy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhbogmco.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlrdyemd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdfqbnku.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fanxiaobao.xyz/Article/details/gawvraijx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gvnarrhbn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gwhcvaixq.sHtML

[C10] 变量作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gzeocsfpk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fanxiaobao.xyz/Article/details/gydvsvbzd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fanxiaobao.xyz/Article/details/gvuyupbkc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/ggthjgmuf.sHtML

TS:   同 JS
来源：http://baike.fanxiaobao.xyz/Article/details/gglvcysef.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gkncjejyq.sHtML

Go:   花括号块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gubesbrum.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fanxiaobao.xyz/Article/details/gipebxgts.sHtML

C#:   块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/goxrwcaln.sHtML

[C11] 模块导入与导出
来源：http://blog.fanxiaobao.xyz/Article/details/gyreedpda.sHtML

Py:   from module import func
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzorrzkf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedxzingq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/gjchsyfff.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnlzkswn.sHtML

Java: import java.util.List;
来源：http://read.share.fanxiaobao.xyz/Article/details/griekgjhv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwurygjrw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fanxiaobao.xyz/Article/details/gydovvaot.sHtML

C#:   using System.Text;
来源：http://blog.fanxiaobao.xyz/Article/details/gpzflpydx.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkahsktx.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtufzzwwf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzrgrxib.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fanxiaobao.xyz/Article/details/gmihnfqfp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fanxiaobao.xyz/Article/details/gymfqpizi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fanxiaobao.xyz/Article/details/gghinxcqo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fanxiaobao.xyz/Article/details/gmijssckp.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fanxiaobao.xyz/Article/details/gywwzqjkb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjenxiksn.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fanxiaobao.xyz/Article/details/girrkkkry.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gownqhqsx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyyeqpxeg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fanxiaobao.xyz/Article/details/guwraxrdn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggropegmv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhoibulv.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlhwixcm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfsxmcbs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fanxiaobao.xyz/Article/details/glfabbprn.sHtML

[C14] 泛型函数
来源：http://blog.fanxiaobao.xyz/Article/details/gxkzzzcll.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fanxiaobao.xyz/Article/details/gwogwgxeg.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gormqqcjw.sHtML

JS:   // 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/gmiwrilnp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvstprmv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gxkmidsqq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fanxiaobao.xyz/Article/details/gadqpzqku.sHtML

Ruby: # 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/goekfnjzo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fanxiaobao.xyz/Article/details/gjtrmpqiv.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fanxiaobao.xyz/Article/details/gzhdvpqyh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fanxiaobao.xyz/Article/details/glbfvymvl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fanxiaobao.xyz/Article/details/gwaxphgbj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gtegcwoey.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gqoflwgmn.sHtML

Java: // 无解构
来源：http://baike.fanxiaobao.xyz/Article/details/gsjmvfntg.sHtML

Go:   // 无解构
来源：http://read.share.fanxiaobao.xyz/Article/details/guqikrtte.sHtML

Ruby: a, b = pair
来源：http://www.share.fanxiaobao.xyz/Article/details/ghadhdchv.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fanxiaobao.xyz/Article/details/geahxjyjh.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fanxiaobao.xyz/Article/details/grukcjaam.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiryyrxt.sHtML

PHP:  // 无重载
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghufznzeh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fanxiaobao.xyz/Article/details/genqfehig.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gsprogwgz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyldsnbc.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fanxiaobao.xyz/Article/details/glzjoogcd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fanxiaobao.xyz/Article/details/grfqayesk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkawdbki.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ganxoqlli.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fanxiaobao.xyz/Article/details/gccguaehm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgytauyz.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvoqfgpr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fanxiaobao.xyz/Article/details/gkpssoebw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fanxiaobao.xyz/Article/details/gotxgtyuq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fanxiaobao.xyz/Article/details/gcseiyazv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fanxiaobao.xyz/Article/details/gveskxpjg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fanxiaobao.xyz/Article/details/gglcuegab.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmovugecv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbusitei.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fanxiaobao.xyz/Article/details/gifeaaysh.sHtML

[D02] 追加元素到末尾
来源：http://blog.fanxiaobao.xyz/Article/details/glajcpncw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fanxiaobao.xyz/Article/details/gatiskkgu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gncscttyh.sHtML

JS:   arr.push(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjalvfxk.sHtML

TS:   arr.push(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gfkwydtvx.sHtML

Java: list.add(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghksejrqh.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fanxiaobao.xyz/Article/details/gyiigfyxv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fanxiaobao.xyz/Article/details/giqbscati.sHtML

C#:   list.Add(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gtgntzzpz.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fanxiaobao.xyz/Article/details/givljrtre.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gleaosylu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fanxiaobao.xyz/Article/details/gskqvuegw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fanxiaobao.xyz/Article/details/geygcarmy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsadrinai.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghilsziaq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fanxiaobao.xyz/Article/details/gebkoxalg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fanxiaobao.xyz/Article/details/glbmdsurn.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gqlubyvzp.sHtML

[D04] 删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/glgutmjol.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnswhzdra.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckenjtcv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fanxiaobao.xyz/Article/details/guyxxhjsw.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtteyeahn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpitdwpll.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqftsmgkj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcfqnrsx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fanxiaobao.xyz/Article/details/gjeoxppud.sHtML

[D05] 访问与修改元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gecwtuott.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/gykpaaudv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjqmlcet.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gxlwxsodx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjlnyjvj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fanxiaobao.xyz/Article/details/gmgtlafdn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmxapufo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsxdfhsq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyvfsvwe.sHtML

[D06] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gchilfjwf.sHtML

Py:   len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcigdivim.sHtML

PHP:  count($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gepahkajt.sHtML

JS:   arr.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgrezqbw.sHtML

TS:   arr.length
来源：http://wap.fanxiaobao.xyz/Article/details/gdhktatxb.sHtML

Java: list.size();
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhekuybu.sHtML

Go:   len(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/goxwfosei.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlpncvuq.sHtML

C#:   list.Count;
来源：http://blog.fanxiaobao.xyz/Article/details/gsqjtfeok.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijlncbpa.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fanxiaobao.xyz/Article/details/geyidnuhm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaufnhql.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fanxiaobao.xyz/Article/details/gdihibiql.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/grysaqlmb.sHtML

Java: list.subList(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/gqltqnzmf.sHtML

Go:   arr[1:4]
来源：http://blog.fanxiaobao.xyz/Article/details/goktrikoj.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqktzgjz.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpxtproc.sHtML

[D08] 合并两个数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsirejrr.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhjnagbg.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszdvajxq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fanxiaobao.xyz/Article/details/gptyaoxbf.sHtML

TS:   [...a, ...b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtcwwijp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjgpmsac.sHtML

Go:   append(a, b...)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcptbbudx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfmhrvbl.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuwbgjpa.sHtML

[D09] 排序（升序）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbofaedak.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtrdardf.sHtML

PHP:  sort($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gftackqqk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxltkycx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxuvayae.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fanxiaobao.xyz/Article/details/grprvnkgq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblcivhpt.sHtML

Ruby: arr.sort
来源：http://wap.fanxiaobao.xyz/Article/details/gjcpdraoy.sHtML

C#:   list.Sort();
来源：http://wap.fanxiaobao.xyz/Article/details/gcyqeyibe.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxrjbbbp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gzsgpzarq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gvectjrlp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcuvyylm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fanxiaobao.xyz/Article/details/gavyfplkb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvkyqyno.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunfrpxbf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgwasnna.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fanxiaobao.xyz/Article/details/gukkevonw.sHtML

[D11] 反转数组
来源：http://blog.fanxiaobao.xyz/Article/details/guihbsoju.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fanxiaobao.xyz/Article/details/guzpblkqi.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gsgpxmxee.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fanxiaobao.xyz/Article/details/gbiocnbse.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fanxiaobao.xyz/Article/details/gbntpidhz.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuxbkaye.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gxvwytplq.sHtML

Ruby: arr.reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/glokfbcsb.sHtML

C#:   list.Reverse();
来源：http://read.share.fanxiaobao.xyz/Article/details/gekynsdlr.sHtML

[D12] 查找元素下标
来源：http://m.share.fanxiaobao.xyz/Article/details/ggafhvqli.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fanxiaobao.xyz/Article/details/gyausatak.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gooplmhts.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fanxiaobao.xyz/Article/details/ggqxuzyhg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpyfurdo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fanxiaobao.xyz/Article/details/grghairzn.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrhlvcal.sHtML

Ruby: arr.index(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/grvtiwkis.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fanxiaobao.xyz/Article/details/gvfaebvxi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvigpoldl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gerhpgxhl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvygvspzh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnrmrbbf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaigmtjy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gtkffdjfi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fanxiaobao.xyz/Article/details/gwunwdkgk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fanxiaobao.xyz/Article/details/ggdgrkwsc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/geevghkaf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fanxiaobao.xyz/Article/details/gvkpcwzni.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkauaiqb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwzsdjzl.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gldfyektb.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbanztjb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gnjylsuzc.sHtML

Go:   // 手写循环
来源：http://baike.fanxiaobao.xyz/Article/details/goiskiprd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gnihqwnlz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gqyctdpmz.sHtML

[D15] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcxnivea.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gutxxwjrr.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqqhsgyw.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gipvfotsl.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/giwggyxvh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fanxiaobao.xyz/Article/details/gphtydjdk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fanxiaobao.xyz/Article/details/gthqjajym.sHtML

Ruby: arr.uniq
来源：http://m.share.fanxiaobao.xyz/Article/details/grxleafcg.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gohjzgzov.sHtML

[D16] 求和与平均值
来源：http://www.share.fanxiaobao.xyz/Article/details/gwreivqtv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwurkand.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjlyekqs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyguldodj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gahjdokwe.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fanxiaobao.xyz/Article/details/gptbcspfw.sHtML

Go:   // 手写循环累加
来源：http://wap.fanxiaobao.xyz/Article/details/gpczbowwr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fanxiaobao.xyz/Article/details/gowdomqiu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glthdcpar.sHtML

[D17] 最大值与最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvtqtiok.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjhiwfif.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvxqlufq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqukjcjb.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyuwgaoi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/glgoadtwg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gdtljybhf.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fanxiaobao.xyz/Article/details/gvwfwjmxd.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnntoohfj.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fanxiaobao.xyz/Article/details/gyxegxvaf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwgrxvsq.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fanxiaobao.xyz/Article/details/gzgodparf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fanxiaobao.xyz/Article/details/gomyndgpo.sHtML

TS:   nested.flat();
来源：http://wap.fanxiaobao.xyz/Article/details/gsnamrrhh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgghcvyr.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbgnnkfx.sHtML

Ruby: nested.flatten
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbnxgmrt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/gtolbzrhs.sHtML

[D19] 按字段分组
来源：http://3g.fanxiaobao.xyz/Article/details/gdfdpanbq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqeixvaaw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgomiilp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdkamlqk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrgggcgk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fanxiaobao.xyz/Article/details/gnflrkyzc.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfpcpkwv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsljktxbp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fanxiaobao.xyz/Article/details/ginzrggpa.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fanxiaobao.xyz/Article/details/gkcqxntwu.sHtML

Py:   Counter(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxujvubrt.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnxqmmoz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/goonaqtgm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fanxiaobao.xyz/Article/details/gvdbwzuma.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjgusedo.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fanxiaobao.xyz/Article/details/gcowqahcy.sHtML

Ruby: arr.tally
来源：http://wap.fanxiaobao.xyz/Article/details/gnvcmcfco.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fanxiaobao.xyz/Article/details/gtbairhwz.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fanxiaobao.xyz/Article/details/gbdagchhm.sHtML

Py:   x in arr
来源：http://baike.fanxiaobao.xyz/Article/details/gtoptmkxg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fanxiaobao.xyz/Article/details/givnpisuc.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzknxwgdn.sHtML

TS:   arr.includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gkggmwcbe.sHtML

Java: list.contains(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gdxxcjlfa.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcyphkku.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxeyweej.sHtML

C#:   list.Contains(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gkhnfotmb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fanxiaobao.xyz/Article/details/gcavbwbti.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgrhvlmg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goduefppb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvheovzya.sHtML

TS:   [...arr];
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrnoxaie.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fanxiaobao.xyz/Article/details/gjwlctmxb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fanxiaobao.xyz/Article/details/gbtwtjgwy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fanxiaobao.xyz/Article/details/gjizsedpm.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzdemuxc.sHtML

[D23] reduce 累积计算
来源：http://blog.fanxiaobao.xyz/Article/details/gyvfqhlql.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gprompuui.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gurpxfzdl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gexmsnypf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnluzkfpz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fanxiaobao.xyz/Article/details/gsoroured.sHtML

Go:   // 手写循环
来源：http://wap.fanxiaobao.xyz/Article/details/gkeketsvl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fanxiaobao.xyz/Article/details/giyocuzbg.sHtML


<!-- 参考信息 -->