代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gzrhlgknh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gmdcmahjs.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/glpkeokam.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gtkpcnxza.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/ggmpjiiyi.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/gstcyurrw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gazbhdppk.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gqrcthbyj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/gaeoubrmv.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gdirmrqds.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/glotpddfx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gxdspfjao.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/giyppnbeb.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/ghupfqoja.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/gbnxpwwkh.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gxchmuqak.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.hesvh.cn/Article/details/gkckfclie.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gobbhqnza.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/gsemfwrji.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.hesvh.cn/Article/details/gzbxuoovy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/glpmbkjlh.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gjxzscwzy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gqspflcav.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/gjizmkxjl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gldzldgmw.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/giyzdnoai.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/gyakbtmvr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/geuvvwjyt.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/gareiczyc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/gvirqytct.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gsijuqgfz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gukcyswoc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/goqhmzyax.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gfgvvjzuv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gorhjpzmf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/ghhrqoaok.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gnlstyabo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/gyeazovsz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gbdbinxpf.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/getupudso.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gxvyujhxx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/glmbkhzym.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gyjidkvzl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/glzaduxum.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/guctqplno.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/ganzgdici.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gbvxavfme.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/gglbnvzyh.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gsvthjeul.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gultygcqj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/ggcegbsxf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gsvqeidlx.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gmwbvdhou.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gvpbiaubx.sHtML

Go:   花括号块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gndxslusj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/guydozbpn.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gastwgoor.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gnsmrgtwh.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/gtnybepmu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gjtyvvssm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gxkbottbq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gwltswxvz.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/grcyptghg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/grpsyguvc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gnetozqqd.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/gbmsdyfvm.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/gpnxddbcq.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gnvtafuwp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/gvaakrvff.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gthwkilcd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gfddvfcby.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gfaullklb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.zdbjq.cn/Article/details/gteibyxan.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/guwuburqt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gzvcbezbi.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/gfeaeshdp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gxqqnekwi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gbezkimvp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/giiwwcnpk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gjxanlqlj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gyndspyhw.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gxfzqhamh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gbzfpenoi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gzkxywtta.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gkismzvrp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gzsjlcolq.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/goznapqcu.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/gvcqqcyuc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gampzobge.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gobofzhqx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/gddjqoahy.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/glkgidzyy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gnpbtgdnu.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/gcztmaglg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/guhtigpwd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gmxgnbfwn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/guewblkch.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gdkrazanl.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gpaglbfyq.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gfqztpldi.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gvulcfhyt.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gpnozufvg.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gxzygdhkg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/ggkgaxhhk.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gsqmaagez.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/gwwebedbl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gzjfnfqya.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/gwbgakkpw.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gsctboluk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gbvvkrurn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/gmxrzqkzi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvbpamxrx.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gbsfkxtac.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gchzeszfj.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gnhnavoaj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gvsflvhyn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gjwgstcme.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gpemnpyog.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gxlradrzj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/grgwfsvjr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gnqaogjaf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/gpzmlhndx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gdajhvelx.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gwdkgsjfv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gxduxdmcy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gciuitykz.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gehbmgcpl.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gcnnsijin.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gjugbjvmj.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gerfvzatp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gtijesrrs.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gjpwypzkv.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gsapmnnso.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gpdqrjhda.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gkjdwbmtf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/gzqterwbi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gsivgzzoo.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gxgsifxyr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/ghafaqnvt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gouiitihl.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gdmamwuqw.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/gyqpozzko.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gactkxnoz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gcqmuehsr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gksgkobek.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gzrknimtd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/ghsobciwv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gnoyzcsdk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gdeqqyyjj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/glyffgcrc.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gaxqxduva.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/ggutruqqx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/ggmauembi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gzbqwzdlg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/giudsttll.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/govnpvhtw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gdgciedsf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gsofgmyaq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gdmceasqz.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gezopfqsh.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gcnohtmsq.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/guchsrvcx.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gvlddwwjz.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gunrpjuub.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gmlzhugmx.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gtwmhwcuz.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gikilggar.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gzulcuqew.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gurjcnmyo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gwedgvoaq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gaqdlntpp.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gjyjlneoe.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/giemzhuas.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gcnfuagdw.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gzmjzonta.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/ggzvchdmn.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gwpdkjupj.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/guooivkxw.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gkpfjnlws.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/grmknnrey.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gpgcnstkd.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/genkarydq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/grgupxtdh.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gbovdvttm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gexdmtref.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gutciggns.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gizqypnkq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gsgenvume.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gfmtbmoxt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gebbgaegf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/grvhyommt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gpuryjgak.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/geegkubgv.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/goalyylis.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gowzojlfd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gyftdqocv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gjltvjpyz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gcaqbzcgr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/glwdhgyss.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gazoavclm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gbktarmho.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gawrhissh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/ggqibzqba.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gbiecsyve.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gbtcvlzso.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gxiohwjgf.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gsafhktfa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gxorxuqvq.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gqgllzqkm.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gmluliizn.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gyzbwlryk.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gpjdgszbd.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/gotviancz.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gajrndqrg.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/giwhoiudo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gndudaxxs.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gknulrhju.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gcqtkvoso.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gtdynaiwg.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/glrwngydl.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gbqoultem.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gefwgipgq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gvjfmgkoq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gnbsbqkuk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gthrazxjq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gggiiaign.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/giytndnle.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gwrpevxcj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gayikiypo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gkcjzaxeo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/guhsmjtph.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gfjyxgapr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gaouvnkjk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gizsvcnas.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gjjdimltt.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/goblhcqsz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gznjffhed.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gbkrnojan.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gdxemenmp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gkrvxiitc.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gevqktkbh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gngfttxhb.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gaxhwhigh.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gviuugmor.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gdtakbcpk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gcldrdupz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gnpkdbfhw.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gaovshltd.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/gnrjyuwwq.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gadztbrpq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gitsnwzuh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/giowbnvkp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gzsuncyfx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gguvmdttf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/glmykubow.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/goxdaioqb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gzivnqdul.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gsksutjlo.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gtlwzmzpj.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/goayvshju.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gjzrkdefr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gimyrawxq.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gbryvjnkz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gtuhwstzj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gzmuvudrd.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gmzjmxaeg.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/grbqrruvs.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gsssabgjb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gmrabngww.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/goqosoetd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/grochitlo.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gqafznxyi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gfotjwjrg.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/giylskmau.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gyfamtdbr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gsdkrgpkq.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gntpehpsv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/guslcgshx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gfkrrlamd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/ghawtbdlf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gmyvzatck.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/geflggldo.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gismaxaom.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gshuwpocr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gxjutrjjk.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gfhlgygqx.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gbenbrarm.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gajqmzjfi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gkhfxnwkf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gcsxrlikk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gpowjgcpr.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gbhhfggxi.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/ggmwlfrno.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gtmzbyilr.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gyustaafx.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gcjhqxlye.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gmodcpgdk.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/ggutqcgwz.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gvwwujmhk.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gowtjfyac.sHtML


<!-- 参考信息 -->