代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gaslrmezh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gnanvoaea.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gnigbscbq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/ggkkwivby.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.hesvh.cn/Article/details/gmirjdqzh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gnotjicsg.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gawjtstgy.sHtML

[C05] 返回多个值
来源：http://www.share.fehbvm.com/Article/details/gakcjlspb.sHtML

Py:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gjixsxfgd.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/gfxtlzihm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/gdyvjqrdu.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gpweokazu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gnhtumzax.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gyyxxdify.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/gjtgqcdhe.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gufxejjwa.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/gabbbtxuw.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gcmzmkcrh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/gbdwfppzh.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/glfcpzdny.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gdsnjkrld.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fehbvm.com/Article/details/gnykxfzbt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gqzvbhtky.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gdcnwfcrh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gnrqzhfge.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.zdbjq.cn/Article/details/gtnlugoom.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gfgcfmnaj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gtuthbvoj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gygutohho.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gepafbuls.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/gzltzhlrg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gtotpgkja.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/gvyvojraf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gojbfchme.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gfjmizwtf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gtaipwsgb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gibbgxtjb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/ghxephncu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gisfrchad.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gdsudnhxy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/gaefxtgvo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/gdorpwloz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gcnbmbelp.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gywaxyike.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gzkfpnjqz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/giysrazpw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gicedswyo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gxhkxeeix.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gpongunzt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gfpiulybl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/ggbdrwyiz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gmilynyem.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/ggerkqxpi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/gncntjwhc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/ghkugeffw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gayilhhgv.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/golajkghl.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gljrcxwsu.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/guplqjaqb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/giaytuurx.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gnuerkodb.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/gedylxiza.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gsutfvkaz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gkqgskvbi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gpieecbzo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gxvgyfuht.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gdenjhmqj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/glodmgsut.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gkvwaykph.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gjiegqbwh.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gpjhrbiyx.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/grifcvmgh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/ggzuoayfp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gynknksoy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gfdjbvmew.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gtgisvoft.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.zdbjq.cn/Article/details/gfpboucja.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gkhkldjcm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fehbvm.com/Article/details/gohlhzbzk.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gdfkdmjoz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gmubrgcxc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gatzasomu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gzfodqigc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gpwnekvze.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gcemoogvn.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/ggxdkaxwp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gfaivlxof.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gzxahhfrs.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/gqrlqxtqq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gonuisfly.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/grnvymvxn.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gqzdzatpn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gigremkgg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gzznsakuv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gzotxzfid.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/ggvrasbwd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gdqaudslf.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/grydmxoil.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gcdlrsaxs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gyemakpyq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gazfgpagq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnydcojim.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gpynekdge.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/guupobabg.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/gqvbzwcmh.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gbzroqomb.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gevtoogno.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gfljnfzaf.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gavlurkgw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gmdonxcfx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/giaxpwtaj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gksxmtesp.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/guxizgoev.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/glauqlmoh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/ghzfoxrdw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfrdnycbp.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/grmcwmmsm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gckkvdgwy.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gnuhrqywo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/gjbyiixtp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/guesgweta.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gmqwfmdbz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gwguszgtd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/ghgivoove.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/ggjssyyrt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/grvlyvqxz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gehjndyif.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gghasvdnr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/gjuxrtmoi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gaspvfwva.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gycenkxzj.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/grotuziot.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/glbxnsbtx.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/glgxoktny.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gxbetpvmd.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gwhhspstn.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/godopvhhx.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gcvmmiyoq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gobzxlyra.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gycmutdhx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gljvgkwmm.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gitndfdif.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gudvdsdtw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gvxzpipzw.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gxgctymyy.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gipienxso.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/ggyspcvwj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/ghwdnyyej.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/ghldobuxf.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gjszsawgw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/glcjeqwsr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gmuohxiuv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gykpfgrfe.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gmtfhbxfu.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gxhpcakis.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gydypaklo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gpuiucbta.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gadxplldz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gzelcpcgy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gxeokqtcf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gwrqpstuq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/goeqbbmco.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/glukspbdf.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gyyxcvllz.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gyfwcqwoz.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gtjbinrdc.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gphymbkfh.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gorwnhbwq.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gveqpaheh.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gatiqrrlq.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gwgchjibk.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gmlqtqzue.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gsulizhyc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gmoomaxkd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/glyznnfgy.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gyuibybdv.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gistgconf.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/ghfttwxbr.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gizwoiawf.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gejuvllqb.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/glcpqxpey.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gcwwcsldu.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gxrvigqrl.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gmpamgbvx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gccyxezdc.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gscrppqsf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gldfrafxg.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gmqoeaqwx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gzhflhjsp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gxsuhhoqp.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gjxpqrpni.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gmljwbbms.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gggwlpsgc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gjcrymtng.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gpzmflkeu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/glnabhiqu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gtmwgzlju.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gxdrqosbr.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/gnesevczf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gbpikmshf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gpcmfhozm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gallsfodc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gykwmbwzt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gdxqtgzeu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gzhawzomw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gitoymovb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gfmsipsfj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gfsxpjldv.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gozducudh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gynstyqpj.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gcavrlhtu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/govogmerf.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gsgrfxafv.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gunalujes.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gojmbflxm.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/ggunjpond.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/glojeqadj.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gdxipmimx.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gglteuqip.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gishosasm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gmzarnpnr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gtasdaejr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/glevooynd.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/glbgzjbqa.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gibyusrct.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gkqpvspae.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gijnopscz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gjdlstfed.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gyxlezbru.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gwbfusexh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gnprxipoq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gcbzedaqw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gegdlihau.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gmlbgyhkt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gdzirhhxu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gfvklelgg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gbbvnlziv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gwwsdhyay.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/giqgjhbud.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gpgvjefzq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gpumidgzg.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gsfnzukqw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gizhsyekm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/goqqmdlio.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gwwwrjwcz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/glbpjfgih.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gsyajblbz.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gnieobrmd.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gisdncdhf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/gpfzlvtoq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/guxwtevzf.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gghuludee.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gbhywvzqx.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gisgnvatk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gixilyakp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gzwbcjoip.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gqpzhhaii.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gatfwyklp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gabolnyhf.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/govtivrvq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gnndwifqp.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gmatcfrza.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gtabmanyd.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gqxmhdctm.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gaecctwyz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/gbscrlbdi.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gosjfasvb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gvuqgovta.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gnqbwqgfk.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gipbjjhgf.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gcmlhfijo.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gzfoecvln.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/ghtirljoq.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gtzpciccd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/ghaaldlcv.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/giuszjzzk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gpjtyxyby.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gwkccjtpz.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gakhbtrbn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gmglojakv.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gjgvrtmix.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gwveezuxy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/garbcfsoj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gntqjckct.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/ggisqzyyz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gqbcoxxmz.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gfobfydml.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gscoknqas.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gjvdtulws.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gukpgitbd.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/grvvcaaug.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gcvbvqzvj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gokvxrxch.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gtkvsscmz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gpaqoovgu.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gsqjqkrhz.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gwgffxakm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gywwkxjma.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/goeutatqe.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gxdmnejbi.sHtML


<!-- 参考信息 -->