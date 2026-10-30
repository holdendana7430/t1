代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gwnnwpxiq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gasudscab.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gbikeerdf.sHtML

[C05] 返回多个值
来源：http://www.blog.hesvh.cn/Article/details/gkjzpcnqg.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gynksdowj.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gzeolcxsu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gjbpwmwss.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gnwnwrmuu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/garlscxle.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gkmadjjdq.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/gvpkwmlzy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/gbvsuoyhq.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/ganejzbwc.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/gtdyauhyi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gwfnsbsfz.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gbypijtqv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gfhspwwbv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gisdwdyjs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gqybucjfe.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/gtpartrog.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gmgogguxy.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/grjnwnxso.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gddemushm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fehbvm.com/Article/details/gphdzxinb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/gsfvzsfqj.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gxldzzpez.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gafyjfnlb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gtrvhhqiu.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gidbvbonm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/ghrlxxzqf.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/ggfstvkxy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/gspkdpssv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/gsdobnxqw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gahqryjhe.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/ghetvrgwi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gdbunnmas.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gdyhtqxit.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gcxrhhahg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/giwwdxgzn.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/gdcgxqacp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/grztsmnrl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gibwrbvwu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gzfsoynxa.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/ghngzaubl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gffpryszi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gsuvxdceg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gbzoulmwb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gohpikrap.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gzprveler.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/giqbfxjpj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gyqokilbg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gvcfmhquq.sHtML

TS:   同 JS
来源：http://mobile.fehbvm.com/Article/details/gwnvkdssq.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/gvivxjyej.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/gudlssfrx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gtmuyqcjl.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/glgcyhril.sHtML

[C11] 模块导入与导出
来源：http://www.blog.zdbjq.cn/Article/details/ghlrsftyu.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gezoplnkp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gxlauopgg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gekhjzawf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gbilrcgjt.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/gmndezgge.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gjpsrihwe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gganpprcg.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/grwvmfpad.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gyoeknfim.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gyvpnxuyn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gzefmuzjf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gewjemoao.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gjefoquls.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/grnbtwcjo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gdakldcoo.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/ggdvlwswm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gqdembyac.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gnvlciipq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gxyaodbwy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gbcesmiai.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gdkbbvitc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gemlpguud.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gkpmqizpr.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gktnmlczh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gxxplevmh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gleaipjzf.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/gevqlfurr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gstvigure.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gtobmdfwk.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/geeyhnyax.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gatanhcps.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gccbezzjg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gieookntd.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gkxxilnrb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gcaoxscvh.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gimzeulph.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.zdbjq.cn/Article/details/gmohrpyyp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/ghwgqgmai.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gbckdppzo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gmtlwvhxr.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gchzolmbg.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gtcxxlnli.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/ghyquuszd.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/gdcgevovs.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gesljofng.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/guscyvlzd.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gotbmnfru.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/gaozesjkp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gajizqvgs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gbcjeztfb.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gtvhedxvt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gtvnouwoj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/gerfkudef.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjlhtdnqf.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gudeekfeb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghsnonzwd.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/ghasbdcuo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gxvyovmqr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/geoqyfiqy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gqupsrsok.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gwawenzze.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/ghfjhlizg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/ggorpvifv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/giacbvdcs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gblwnuygq.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gdsvpdfmz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gllcfrqke.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/golomoyzf.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gjwrmzdzn.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gwmkavkxv.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/ghfuqhqpq.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/ggqccmteh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gpwcqyvee.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gwimearsi.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gaobkijcz.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gwnyeymxg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gmhipqoil.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gxxqyjtpr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gbzyuhnqs.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gcxszcfii.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/grozkkjxv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/ghzbgnits.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gxnicogvr.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gnwgmuxzg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gblbiftpl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gyouvkupp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gcfkaqrrx.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gbgynxbrh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gqhyrphrw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gsvimfbpq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/glpmsvrtt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gpxmmmder.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gjtvtbhjj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gcvlgoujl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/geslrgbsz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gynbgnkfc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gvtmrtnyn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gsbcoqpxc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/ggvyfogyq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gxmgizhin.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gpfzkotbn.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gvtfaxusz.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gvmojvges.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gzizpxvsh.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gvtwupyer.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/ggjrjfdpo.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/guksizfgf.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gliuslsxj.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gxlxoximq.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gdvuphmef.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gvvlatvpk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gmgtvllvo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gemknkljr.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gainvneun.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gycxbzvnz.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gzzkftxlq.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/gnqamromk.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gtjvcycxk.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gywzjapaa.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gwdcadzwg.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gphiqtaby.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/grvnagenx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gdjzbndrz.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gpovcuazb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gioxdwxyx.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gokdutahk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gdplovsqn.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gwaxxjxdg.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gmxnurbfx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gvxvlliid.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gmzaiwuqo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gukqmpaxy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gwmgwzigv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/grsyjgdod.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gvicrxtrl.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gavyccmdi.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/gprnrqrmo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gawaagmzy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gzzltrxqj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gxfqhjytv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gnngjwkap.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gkqoqorbm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gqzlmhemu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gbaklrdvr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/ghpdhjoaw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gdjnwntwf.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gsaprkbvu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gsgnxsmap.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/ghoqgcwyy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/giaznuckk.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/grisnnkml.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gmrishwwp.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/giigqxloi.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/glfcrxloc.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/glfmopulk.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gfyrnghmw.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/guuoenkjo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gtkvrrodg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gstitgpow.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gnihhpdpm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gyurchgwc.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gbmaydozl.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gjkmxfauh.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gqmdhgvvn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/ghoghztkj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gsinhfdfg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gklswzhwh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gqxfzvjsr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gympjmwnu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gvrnjgpsa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gdcpurfsk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gonifzkgy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gnpxdkuwe.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gpwftodai.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gugbumyvn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/geuszmcmu.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gjkylszzh.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmqxrncyx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gvidgkbjo.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gppghtkoe.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gerbptxbw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/ghkxducuq.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gndwlyfvg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gpbyaufyt.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gfhywsxyh.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gnxdclyrb.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gtyfsosak.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gbjjviufn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gbusdwmmx.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/gwjuqwbpw.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gpbgunlml.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gnfpmfdje.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gdglublhn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gdktpextj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gvkfzrlan.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gpsmusbgs.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gmtmspjfn.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gldferkcs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gczospjln.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gzidliwde.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gcprubhbd.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gzarzmttf.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gfqmyeorw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gyysntpoj.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/ghvcudkbn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/ggrbuduvt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gsnsegzsx.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gbczgkfit.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gewkdxgnr.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gpmfhdypp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gdrvwkrji.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/glhybycdo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gsepdtqmv.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gcngexeqt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gnernvxtj.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gwhanbnis.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gfcfvnuqm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gktjeocwa.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gosaially.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gdcixbvij.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gqpgncqdb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gyugbpwji.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gxpjlehmh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gcuvnyxcu.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gzcswnjky.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gkahpqvqi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gqqbvhhvi.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/givyqzoat.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gtxpzctel.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gbkjjkmlq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gilnvllmb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gnykrmeam.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gkldoacmn.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gicgbcdyl.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gycwdliik.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gtjrlqukl.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gakhhhnam.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/glqehqdyc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gamzqykeh.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkmornmws.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gclghvgaq.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gsioltvbg.sHtML


<!-- 参考信息 -->