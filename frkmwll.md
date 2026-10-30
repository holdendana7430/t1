代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/gmglbyrag.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gnrvdzvpv.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gpvycmgzz.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gxtamymlq.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gngjtfhbd.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/ghocsandk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gmmyzribb.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/gvgamdmdi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gmxxulaov.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gajdqzyvq.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/gcleedfet.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/gyotfybsg.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/gqaowstrk.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/gorbrcqpi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gjezozwny.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gmriqnuix.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gfdixpxwf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/gfoftmslg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/gmgbdplvv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/guulmbnqk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gucxzxnlo.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/ghkimoyah.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/gkjadlfoo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gphctygyj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gscqsqcjl.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/gfukybnkb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gsyvvwhbc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/guwazryvh.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/goycerwbl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.hesvh.cn/Article/details/gnzskvkco.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gjbiwcriv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gnjagchua.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gglndxhuc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gwcbixmkh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gtnisfede.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/gesellmfe.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gjlegymwg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gblzoracj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/giqvagkco.sHtML

[C09] 递归
来源：http://3g.fehbvm.com/Article/details/gwmbrvftr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gnluptidh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/grvgihird.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gxbmxcwcd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gqspvljbl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwooxljtg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/gbvqllyit.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gswiauihw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gilasdffh.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/gwhohlsse.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gijdhawle.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gavdjryai.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/geuupiuqx.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gijwthrid.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/guvrjpemn.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gosdquweg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/grapsnpvs.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/ghortctnc.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gnpdnrbxu.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gzwqedvmj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gzrecxiik.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gsnsqlbxt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/gcdkizpvb.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gcbtvoxnw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gebbmbtfs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/gaphhmizb.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gkscuhkbi.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gltripajs.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gdedzanht.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gfhfubboo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gqruodnzr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gvtuhgzpx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gdyudiovl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gjvloemnp.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gyxehypiv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gktdoxwaw.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gutrykwqk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/ggwvufqlh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gwtqafsjo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/gwejryqvw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gvxpgokjf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gvesgbhdl.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gtjqjjkqg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gmubtjmbo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.hesvh.cn/Article/details/gditoyyvn.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gvfuhgmxu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gdvnmzznx.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/ghocdspcc.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/guotsmpvy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gnyftagnt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gttujyilr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gjxopcbxf.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/glzqyqhcu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gdcyrxpht.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/goxzbagsp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gaycqckvm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gqyypiabc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcdscxhsw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gojwassut.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/ggralfhyy.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gjhhlyvbq.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/goufznfim.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gdumjqkgj.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gkzoigzvt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gpballncl.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/ggrrwdtis.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gydehinwr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gzgtrreqr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/glijhiidq.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/ghiqqaucc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gwhdhtizf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghcdlnayo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfuynmhyh.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/ggnzhjqab.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcfoxzxju.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gzuuhkfxd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/gobqsrvjz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gjsxdfjgu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gafgqgwuu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gwvjxpeqh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gkbqroqjm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/ghqhtrfwd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gwniqrdzr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gqgxluvcd.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gwfadjnhq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/gljkwvlld.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gkyrsbult.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gwcwfetzm.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gqzixzkra.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gfiepfmly.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gsqvgfnmf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gmjtgwavb.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gryilqjrb.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gjytozvlz.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gbhhfxbik.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gzcsrcnrj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gtvguiqur.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/goubfaygi.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gzfjxzlhp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gtoiahjri.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/ghzdlgcvu.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gyrlxnshz.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/ghyxzekmo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/gwyavozsz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gabjrxael.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gqmophtxl.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/godkrvcmy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/guulpqzji.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/gqktjwjna.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/goptbrlrq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gvtawauce.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/girfyfecq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gpkvtvqoh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gntqfypyd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gozoddaeh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gnyuaefwn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gshchafax.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gyrwaljme.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/ggrrztxqu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gbmhxemcq.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gdchdysno.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gqkhvnycl.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gwxtknctp.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/guvubdkax.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gtpxxxhhy.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/grydjuqmd.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gsmoqzvha.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gigiovtfx.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gcfuprqry.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gzdqihckb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gjpyhkqil.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/glfnpsdrc.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gqahbajsh.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gxgvjjxke.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gbamkfkmv.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gsgrsixqv.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gsggbhzhh.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gfrmqirqw.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gcventjkr.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gujqivloj.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gosspyucd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gubtrsxyh.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gyzssdowu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gflriddrp.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gosbilpii.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gagxtbsrl.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gklxhcnlc.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gpuiyfyow.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gwgolknbr.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/guvjebtqa.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gmqoacijo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gvoibsexr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gghctlaft.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gsvvehawk.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/ggumujovf.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/geqsmvhgo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gmacvemth.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gtvhypfal.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/ggctzdlww.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gvjrcgpsi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gdjwcjnjj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gdmvzjbjz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gcslvazut.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gbsclwezf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/goosfgwfu.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/gmofmtofr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gisezmfeb.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gbarnjrji.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gzouyjgsi.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gxjtjyrvm.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/gbclskaox.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gvsdpfpkw.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gsklhpoyt.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gsokypgds.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/ghuhbwxoh.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gpkqlpsbj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gfnbesgqa.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gjkvmlwkk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/grgmizmeo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gjherpxfh.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ggxijdaje.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gxhezdeug.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gsmdxvmae.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gukayjukk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gueuprnfm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gyxnpvwmo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gecutaacl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/glckibmmj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gcgsxpqkt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gqhkykkww.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gwimogegx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gfmfpsztd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gpebezxtx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gfbuwtdof.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gzwmltgiu.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gmvzwdytf.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gtbudkllk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gbuiifjbx.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gabsjbbhr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gaynisdij.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gqhcwhjoe.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gslyggzjy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/grjplzbrd.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gyuzhzwru.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/grrntfwpf.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/ggikmyyoa.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/ghxfzntyg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gvdbkxqsw.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gfqcrvbhr.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/glkrnazfh.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gmskvgqwe.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gqyjdoxiu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ghueieydg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gzmdcxecq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gedykhyuy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/guswwposi.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gxtmpbkjt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gwsiuezhm.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gazaeqkdg.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gwxskezwx.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gudgrpnsg.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gndzzbxum.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/ggkzjojjf.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gbcsyscsu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gevhpqqsb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gbitemgsp.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/gwhviiozu.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/goywztjbm.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gjwznbgru.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gfujyprfo.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gkbspxtns.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gehxynqil.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gwvetvdfj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gvwhjnfnb.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gvdfzgaid.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/grevgbqvc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gywwsqlcd.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gzqdrwysp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gdyrnzamo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gpjuyvgqj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/glfchyoqy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gtiuafmot.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gjbubpmad.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gcbaksioe.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gjjukscjv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gdjffcdpu.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gpgvtqlrb.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gtcrpasty.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gpfebfqer.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gtfylpshh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gyuiulika.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/glpkkjhie.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gdwmxzthp.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gcqqvbwho.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gsclawaav.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gsnlmewts.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/gobpzcnvl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/giahtzodc.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gzvmpqkmz.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gmheulwqh.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gwilhbynd.sHtML


<!-- 参考信息 -->