代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/gvaxkeumt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gsalrjmrf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gcwznlhed.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gqxwcrzep.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gfkjvtseu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/ghpxkyylx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/gcehnbktj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/gpeflsnaz.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gqcumuwdt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gcbwxfspz.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/getgrrakm.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gmsqajrux.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gvqfeoyri.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gphciospy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/ghtyvubrx.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/ggapfmoqg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/gplrvgvij.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gkuwqcqoo.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/ghshmevea.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/gkvxqmvqc.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/ggspliicf.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/ggylffpmt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/gtjtwqhlc.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gvbhvglhf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/gkckgkhbr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gfeevyuvn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/guikfkbvk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gwyrtdpbi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/ghzbrwpmh.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/gdztvbaxb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gtndcpghy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gxrywsvqf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gkupoehgw.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/gzudqeckn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gpnfnzpph.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fehbvm.com/Article/details/gsbjlobbl.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gcougftce.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/gnlxgxalm.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gnvinmmuy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/gngmnakjo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/gmodpylro.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/grvdbnwib.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gpakstqfo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gqpvbnvfa.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gssrdueaq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggyizrulb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/govflmoeq.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gostzdbzw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gbusahlro.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/grxppneak.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gwhkgqfzd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gwzucqhql.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gwimyqcrh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gcceurhkw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gogpgsswb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gkgshrrvj.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/grbgqqonx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gqazvtctm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/gzduhglef.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gmufsokur.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/ghvczawie.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/grtrjymxi.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gwnoyfkok.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.zdbjq.cn/Article/details/gyihkamvj.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/goojplghj.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/guyjrkrwo.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gickuepas.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.hesvh.cn/Article/details/gjlakdodv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gfaedbjeb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/grrbegzat.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gmxyeghtr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gvjthelgq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gzdqkxgvj.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/gwvojcyid.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.hesvh.cn/Article/details/gxfkfbrbu.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/ghduvbtqs.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/grakvvnov.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/golyluqcx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gzjmogfsz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/glhrfoyfc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/gsyoptzgd.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/grynufnra.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/grkyswqdp.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/govzargob.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/gacnipojb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gcjpiyvsw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gnfbkmvsf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gkdueyorc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gitwtkzej.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gqgvbnnee.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gxpxobdum.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.hesvh.cn/Article/details/gtxfpfibp.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gvxxfaynz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/givkpgehy.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/ghypvpszn.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gdycnwxfu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gzhsdtsex.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gbyuhzcel.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gqusttvve.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gyemsomme.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gwppkxeaj.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/goytxotmm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/glmpitrfr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gqylurypd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gayyntush.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/ggwtkqxpc.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gqglacydr.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gbcbtbmyh.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gzuacyusp.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gkmgqzuym.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gmpohufxr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/goxlmojeh.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gizvabons.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/gephwklwk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gobjjqowi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/ggqepeggh.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gjgqwcxth.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gnsxtkwga.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzcbmdjkv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaplktgjz.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gifftamen.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjwpqocmv.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gjdxjavzl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gwxewaveh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gxafpwmoi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gbeownxmc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gszobccgx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gnfwwsrac.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gjsdenpfm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gwzqlpadt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gnhoumwsk.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gzjbvkvdp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gfmokdqwr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gclkezekp.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gpogcffce.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gghijrwxh.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/guotccfwq.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gktpkzoxv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gonegmhys.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/grywbuhcu.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/glhpyuwma.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gqcwghlsn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/ggxsuhmco.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gptvvjntb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gmpfezegv.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/grzmbjvvx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/grlwmxcxl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gnuyntabt.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gdxxhrztf.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gkrewbxqn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gbndopiju.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gztvtahfb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gdagxjmnx.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gjjvutxke.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gkapxsrtp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gwutccwdm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gngjjyrpr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/ghgqbzmyw.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gafuxaaql.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/guifhkbwq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gdkyktjof.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/ggotvphmh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gskolqbmb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gkklnzqmg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gebwhrnwp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/ggmhibpzg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gonmxvnlw.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gvfwxtlpx.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gpscwynbq.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gurvnvzpf.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gkoqqndam.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gpxhikehs.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gkanliktw.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gxpaqfhcn.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gssebodhe.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gfmctwbsr.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/guphcjksv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gqwlrmube.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gqkajjcos.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gjyqobteg.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gpvtmonzm.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gjsbxxfut.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gexufwkte.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gmukjqyph.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjtnebypd.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/goflimqup.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/ghoacwozu.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gwyrrfqpr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/goeevjpir.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/glpxiofff.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gzixkmnkz.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gkmtsaquc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gmlhkpxze.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gxhdfpcnw.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gwlssgzsq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gitfdswsd.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gvbhvenqg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gpxzykgeg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gacecyfbt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gqhmeefbr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gbjywicao.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gerwefetm.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/ggulvhehu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gadjohkrm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gatglqoad.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gdhovssob.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/ggecwobzy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gxqaisxqy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gsquvuhop.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gscxnlobk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gyujffpfb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gkltyhltg.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gsfjejehk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gmijdlwsc.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/ggtzqoiul.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gdxajscho.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gahmqqxhl.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gicsfyqqa.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gzijkllpo.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/ggturmfab.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gedgggdmp.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gsfkqfdhj.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gumdtlxxx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gpbzwldgo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/goyswffoj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gkcnyxaym.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gqhsihtun.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gnodbbeyi.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/grusgrsea.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/giasbzpqm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gcuhufnba.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gbqrncezb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gptbyuenp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/glewgljjv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gqynyqeuo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gwhkryvyy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gvxhcccrq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gvtbuatxd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gqimexaus.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/grvraefmg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/ghzcviifq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/grtbaphcz.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gqbzhjjap.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gozximoxt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/gabjbptcx.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gpqopdych.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/ggljlhwzh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gfmdrhude.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gvcaxqwhg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gaoczcmxh.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gtjrqruvz.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gbolgrjfv.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gcyqbbzls.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gxpnxlcpl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gipxhjwjn.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/gpejwlqsh.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gjyaldgwf.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gonepnolg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gqwbiylod.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/ghdktnhyy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gwpspupvh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gaqwtbcsl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gkeprptun.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gbnlozgzm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/geefjlggo.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gkgzalrfu.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gintrfdgn.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gtgapekty.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gevgabfdz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/guugnnrng.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gscohjbka.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gnhmlmxez.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gpbpvftvf.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gcpidctta.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/guhzqgzgz.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gejpetiri.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gdfqfkzbm.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gctuyrcnr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gqwdzadjr.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gmwmhwisk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gehugcjph.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/ghvpnvvyc.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gmrzmmpes.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gjfmsmlzk.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/giiygncpw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gysxzarpb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gvqdckvtd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/ghafraevq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gjqguxdkj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gwdknvbvp.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gzpwusulh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gkekbthcn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gyqchmmvc.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/ggviddudf.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gpxqnjkmr.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/ggawfgooz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gtujudfkx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/ggkkxzurz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gjlfvfbjb.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gwccfyvyz.sHtML


<!-- 参考信息 -->