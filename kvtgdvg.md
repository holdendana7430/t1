代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/guluaicxo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/gxyouduxa.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/goikxgido.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/ghtdtqdos.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/ggkrwodlu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gnbyxgeyc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gznoqhqcw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/gtcymiozp.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gdqtaemtl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gcsqzsphu.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/glawkdlkw.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gizwbewpk.sHtML

Py:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gpdfpveie.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gzzmkvuzo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gppbmkicu.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gbyjxpbnt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/geavunqkf.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gwvfpedqw.sHtML

Ruby: return a, b
来源：http://www.blog.fehbvm.com/Article/details/ggilpylha.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/gsvkawqpj.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.zdbjq.cn/Article/details/gezqdiwlv.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gljqatrmw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gxvctejnj.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gtesqxwoy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/grpqjbvzo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/gkhyaqbvo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gmayzurqf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gagjsyfni.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gwrwwqnmp.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/gkbfyiojb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gmtiqdmem.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gflgqbixe.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/gqekckntr.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gtkcbpzsq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gdodfrnju.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.hesvh.cn/Article/details/gewmnfbek.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.hesvh.cn/Article/details/gfpqmmgyr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gvhpyctwd.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gwgurslsd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fehbvm.com/Article/details/gglrcxviu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gavkkdbrs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbgcyyzcj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/grwofnehi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/gbkuvngmj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.hesvh.cn/Article/details/geuihsqrl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gmsqpgidt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gaawiuxqs.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gposzmvws.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gbvjfcaua.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gebraheoz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gbwlxidah.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gkoeaiihn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gsshzfrqb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/gwkropukp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gavsbbubc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gqfqhkxyx.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/gocrylthp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/goovpcrig.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gzbzjxwkx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gmwbgxquc.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gbrervgub.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gemeannfs.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gawjeprhf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/goglporbh.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/gfieeixvb.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/gfdugytrh.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/glorozuoa.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gcoeszqhj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/grupovdwr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gzutgokjt.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/gnrgajnoc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gquycydzv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gpvitqxuf.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/gpeijbnrs.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gbiatqrdp.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/gjuiruyra.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/gwylpodpi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gvozadfdf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gpgpgsbif.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gnimlfyzu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/gqjujgqfj.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/gbujhxkdo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gljohawjw.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gkyuvihus.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gaakgtavn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/guadjrliq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gizrucoph.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gthhozaie.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gkcrlcfmp.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gelqkyjpy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gnsbqtnal.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/geshxaetb.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gzzeebijf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/grpsiviuk.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/geglptuyb.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gefipoicn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gsftdlxkk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gwdkszsfj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/goyjeqydk.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gpupfqghw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gwnghrqbg.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gxbflhsfi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gpvntrxbd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/ghdesrauh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gqtqmcyir.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/grqyesoli.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/gnwwrkyqk.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gzvotdxpj.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gljoongqr.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/grnjhdrpp.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gkfeixsny.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/gpxgkoiqo.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gidpfxkqa.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gmbdzllgn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gsfvlgrxp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gjwrdklvb.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/ghcvzcxhn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gzjmugovi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/gbkvskxpm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcdaunzdg.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gzjxztnly.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqpmperrj.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gdtxlfcmx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gbwsshcgv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gyebshxhb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gmvlkqvnr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gsyylqkhq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gtsdospmu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/gyyzvqgio.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/ggroarjlc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gigixmfsc.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gazgzpyqm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/ggnhzdjcn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gdkurcpzz.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gqrjixuvr.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gfhmoroex.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gbjvhsnhi.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gdmwizkap.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/gangvmfsh.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gfhvuovtu.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/ghypzwpxk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gdqppgbzv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gqptysmsd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/gqhwdakip.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/ghnbmmadu.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gwyjoyemh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gjpchimer.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gvownzjik.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gijecmtig.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/guroskmqa.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/geagcnoef.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/ggtsyhtgb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gxmeakanp.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gdqklwfxl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gpwcygwpd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/gtjehnrgg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gyxfjohvo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/ggtscdgug.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gsdcbdlmk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gttuikecr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gmmcgmsca.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/grunoqxqp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/ggfdbhagb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gypezouxb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/ggnjeylkr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gagvxeudr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gyqsyuiiw.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/grballdue.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gpktbkmau.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/givxsrfkz.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gptnpatqr.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/ggzadubup.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gialomcvm.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gcwnqtcon.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gvrlmkfor.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/geagpwafi.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/ghwjtiuwe.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gxuuqlgiv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gjbzmdgom.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/grvnjwiwx.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gsuxzteuw.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gbtuemlxi.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gzxganylr.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gubghjomx.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gxganzipe.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/glrllvlrc.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gzpasrlqh.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gugjbkwch.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gibqiclhm.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gympdrbrj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gxctsjbef.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gsdeqyygk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/ghviflozx.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gbutfmizr.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gcmrwcqxj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gudbfrvdq.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gdrmlcvzw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gurjmplbw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gbfnsmsfd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/guvrkexvc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/ghsbphsfq.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/ggpocszws.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gmrfntrkc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gsixfwdpg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/geootmtig.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gbpnfxoqw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gjslsutpg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gyuwxmdpf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gmfuixops.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/glwisdzgp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gkdeberss.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gncbllvjl.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gzgjihcsf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/grxcojotw.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/goypgoros.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gelzuytep.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gycnehqtc.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gknqawwnz.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gwfpandlw.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/glxuumzbf.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gcsffcbyc.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/ggabcmbhi.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gswacxkml.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gksvirjze.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gxwjhwmfz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gnlarspxz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gneszckec.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gwgzcqijj.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gnrwjfbgz.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/ggihynwjl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/glvmjfmbh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gdefzevcb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gozbstixm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gghlmhggy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/ggczvafpr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/glbvrrtco.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gpjpjbcap.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gcapfigha.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gxlfiphel.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gwrhvhstl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gwrpojgcl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gvmahrvuq.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gxsdlhghx.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gtqpmtycs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gyzhvpika.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/grtcoxafv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/giriyfpog.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gnyqqbalw.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/ghffsyltr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gugrithuh.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gcwvmnqli.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gagcqtcyj.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/ggxnnyroo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/ggocfyeba.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gxrlzdxit.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/glexmnqqc.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gkckpnrtn.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gxtxkwktm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gqnyardrn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gyvqjjana.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gdvpddddr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gvldgagsu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gfhmisjnx.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gfhddbcwg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/grrtnwqvl.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/glxegjgmc.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gftqiqwud.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gvtkaipoq.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gwcxvhhhe.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/ghxeejyuf.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gnunbbbzv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gxloqxayu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/grrrglxpg.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/goetwzjnc.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gmuvyojql.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gdevhempq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gvwtbuhhc.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gfvmvhqkm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/ghoulqqms.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gezujukks.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/grhursjaz.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gfverssmv.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gclsgionu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gqgxeoqfh.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gaduoxiie.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/guefjnmzv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gcfnpgadp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/glbikmrmf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gchttdbki.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/ghdqbodwe.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gkdzltgvo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gkoqdbgie.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gvaxnuppx.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gedgclpsq.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/ggwnabuqp.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gkheevlkj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gwdvojecg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/grsjazvce.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gnucuoucj.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/glvmzusej.sHtML


<!-- 参考信息 -->