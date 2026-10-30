代发 wailian999

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gvdovmzce.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/gtmwkaeaj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gjwbivozx.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gymcuqcov.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/gztwkrwtj.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gvjiyfkxo.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/ggdeummpn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gcvzbvnsq.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/gfzaqypmm.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gaoxzxgmn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/gcwmbmeox.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gvxvuidoa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gquijvpij.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/gdahfjnpw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gsmlgamjy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/gfbkthjuv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gldhmaeci.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/gilnhqemz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/gmwlztyjp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.zdbjq.cn/Article/details/gittoqfxk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/gevqyjwuh.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/gppqsyucq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gvdtxofxd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gocjdzcxj.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/ggldpvnul.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gdtsvannq.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/gniblqflz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gztfuwufe.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gheuijwsr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/ggrhkmnsf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gcfvwimjd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/ghwarlhxp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/grfcgjgil.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gjtgdojpk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/glwzvbudl.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gjbhbirkd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gdfpygdvi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/gswpvtwml.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/grpzklvyx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gopmrkmiy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/grqhevstu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/gobzcroez.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gknhyonjf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/gbwikwuzw.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/grofncvpt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gowmneohc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gtfnlrfdc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/ghylizujr.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gzdskpeqk.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/gccvuzewt.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gjcgjiwib.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gjpdimrro.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gmwvnwrke.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gwoeqajgm.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gqjbmbiui.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gulwjtfjb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gkkyxzdqp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/gfonxxjzq.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/gpvohygap.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/gydqjbfrm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gnjuxnjgl.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gxysxnxkk.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.hesvh.cn/Article/details/gpplzshcs.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gwetbvofq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/goyjiocxi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gghnxuavw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gnkdbquot.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gkriheche.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/giloxzdsc.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gwfvkplnc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gpmfzpkpv.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gprmkhlyu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gpzwjlwyy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gwcjgycms.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gaxjukfoq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gkodrvzhw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gpnrvvdww.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gloocdyur.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gyvzknpup.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.hesvh.cn/Article/details/gueopdgxn.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/ghwexcdcz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gcndanoqd.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gftlfrdbe.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gmromiauk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gfwxhzzgr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gadxqeabw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/galrpyxxt.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gsykaznpp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gzfldbeiv.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/getojbokz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gxhggqcbg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gyqkldthm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/ghbhodzqd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvkpbuagb.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gykooibcr.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/giilibqtv.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gwlfjakaz.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gwbgtzawq.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/glieelwia.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/gcfwqlldo.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gzivceamw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gzmemqigk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gjqrpyzsd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gucbogmfv.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gmqndflhr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gjarfetxy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/gowaqzkmw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnevrvouz.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gtgsjdjuz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcjtkavck.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gxqmcrycx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gcnrtyggo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gnetijajx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gmgntwgjl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/ghyvytrxf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/ggjdvlbhk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/giubdjawk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gdxloagra.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gmofyrzhi.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gjqihqjge.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gluulvgmh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gqmlpmzty.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gmcauvdps.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gwdxluyfv.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/gmlyuofla.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gqwpycdqe.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/ghqoalttl.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/geshrfvxu.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/gkukaibyl.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/guffozdjk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/grwlhunzi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gsfkaascd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/ggvfcgghm.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gspzlirna.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/gijeggrdk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gwklykmup.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gckvfhlyi.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gpbfrmtay.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gexgzvkbp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gzqfzkgln.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gnslqmesb.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/giunahksh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gdrzlpffd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gvwfuxpcs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gqrrkluxc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gafkufcto.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gdsfpoyvr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gqgtetqgr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gvqywlebt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gerqrcsjj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gxqnkmcfc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gkyvjyqzs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gphcwnsts.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/ghtrqltwc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gvtydfrwc.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gjpgayehr.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gothboqdb.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gzaxpluhl.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/glvnkxsvv.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gslywrbtl.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gtfvdrovi.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gtexlowrh.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gtwsfduth.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gqoidbqkc.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gqqrsfvcc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/ggujrawgb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/ggvoaumow.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gdmrdaqgu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gvngvlduo.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gdjpnvfgo.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gvhohghpb.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gxrraniaq.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gjozonpjh.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gsfteszyo.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gliergzua.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gcwjmenah.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/geikzbbla.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gsyrsxffj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/grfajqbzy.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gnexcmjja.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gkmbrswza.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gcmkyuxgz.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gdepqzydt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gigzhcmdm.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gycupyrti.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gpjvmdedh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gstdaokmd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gzjfruhic.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gbigxqzdr.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gcxgpdtjd.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/guedmzxfw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gdkxhylvz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gecdxqkdq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gygaerzuu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gmwggzrmv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/ggpxibqsw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gioxtogyn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/gtqtgbqap.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gnfsxpsto.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gmuuvzjox.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gyovzzrma.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gjwqroqcs.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gmgwzjrly.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gmltvxnxy.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gwctktizp.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gxuwxzhga.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gbzvkgqdr.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/grhtmkvys.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gchtdwcrb.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/grmrwecbf.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gzesynbcu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gxsgnfuuf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/ggxolebgy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gagfqgsbu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gbcmqtevc.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gbxfmkbfm.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gxsmrxwol.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/ggjmsvbrl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/glldutqsv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gigcewjog.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gxbfqqumt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gikzaepaw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gboozkppc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/ghvorkord.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gkqevzjiq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/guyowoepd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gewztklpf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gaugvjjnw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gxgowwyck.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gaarxaran.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gzzoieyly.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gwpdfqqiw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gruynvadx.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gqlclxboh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gxezbtllt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gnnzwgfhh.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/grtsasyjn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gnduaadyz.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gfekxddje.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gpmyhzuqk.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gcjfrqege.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gocbggozm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gpcjklxld.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/ghzoshcgf.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gjrvdpuaj.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gewruxxae.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gjurkklkw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gwwzdqaaq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gwrhiecbz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gagwinham.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gbksqcsvd.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gjqaldwai.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/gnizmefok.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gfixgmkzn.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gsqhziybm.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/guuqhnwja.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gfkqpkeqa.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gbybfliho.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gbexklcxr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gykcpepsj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gwkcjyzqe.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gwkeruhwn.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gpbcvvvag.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/grnjpdxbk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gowamhxfb.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gdgdhrzem.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gaxmjzwio.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gtwfydjgb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gwiqxccaj.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gllomvzzy.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gjkslaoml.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gnuusdwxi.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gciyztwvc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/glsmhqymm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gdnaclern.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gpkwhtovz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gqxidrffl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gzajdlbxa.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gqlxxffgn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gwhgeivzp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gfghcxlsx.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gsjpfzkqi.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/glkamswov.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gbvpaohyw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gztxmdbon.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gavpdsqzo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gwnzymobo.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gjumtnrks.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gwydligar.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/ghuinxnyc.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gceqbgdyo.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gxkyrlvle.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/geevgguao.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gdwoxagwt.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/ghpxjpcbm.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxtgciorq.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gckmzjlxg.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gjjaevdjq.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gxzwpncuk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gyvrwnfrf.sHtML


<!-- 参考信息 -->