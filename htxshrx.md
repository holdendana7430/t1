代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fehbvm.com/Article/details/grwhsfkea.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.hesvh.cn/Article/details/goxobuzrt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fehbvm.com/Article/details/ggwibdzfc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gutvpuyzv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/ggmzigbqh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/ghemvdhvj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/ggjrwxabp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/goywrmorb.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/gkdeimxag.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gnkofctlg.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gkubbxrrm.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/ghdnonfng.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gheeldomz.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gujzwpvbs.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gyqcwcllf.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gcgibxije.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fehbvm.com/Article/details/gupaxrsbr.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gwkflfjxy.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gbtppozfr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gexppgfak.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/gkruwprkf.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gzmnytnvb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gvuaajktk.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gbzhcnugy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gxdyasghe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/gooxtzisv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gbknixotl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/gfjkysuys.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gkieentby.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/gaunqzjpz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gprivorfe.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/guxzdigqf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/gycyxhjba.sHtML

TS:   arr.map(String)
来源：http://baike.zdbjq.cn/Article/details/gjdrihlpg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gltuhsqpm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gbwazefpr.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/gaprxrhll.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gbotxgwlx.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/glvvycatg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/geoorxoqp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/gxvnwzxuo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gbsohdets.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/ghutcgnzj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/glcfnjkyr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gsgubfvsk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/gynacevtv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gstusdpre.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gtnrxweus.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/ghansrxgk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gxedhjkui.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gxzqxaevo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gcqbxoays.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvmqixool.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gmlrrzthe.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gvvzdhdjt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gndymonaw.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/gwbuehscg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gvjetkwrz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/ghfaitiyg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/grbpwkifn.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gyqbfiihw.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gwsvsxwrs.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gzoensrkk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/gtbqiefrx.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/giohuzpee.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gfhkgvfzd.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/gqobnqxrq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gukikygqw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gbpylayus.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/gdxjijpzl.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gnrxftyef.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gxxejitwr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gmafripsn.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gswmcmcty.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/ghgarmbjx.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gbjybjhbi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gpmxeixwe.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/glvrjuvjf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gcuwgznwf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/gydioezkt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gajdlpqzn.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/gatbacbwo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gqlnuuksl.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.hesvh.cn/Article/details/gimnxqmly.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/gtxnjpbyx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gmimpuezw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/ggkuvcvpv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gdqbvakjp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gchzvrtom.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/giuddgaxu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gunjexrcc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/gfupvvuwy.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/ggtwdrwmx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gvmirwfdw.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/geqjevamg.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gzyvpixpx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gpizubohj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/grxxrpunz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/gnrvakypj.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gvprfaesz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gtqstyxpl.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gqoayixqw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/gzxnrkrrp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gxmvuuitg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gwlwryiew.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gzdjwetwx.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gsvhkzwss.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gheqaprei.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gajouiulc.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/gkuufdtoo.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gbtmihhqs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gztpyxgag.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gjsytjbbs.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gydnvlrkt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gwbtuxwum.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gtnkcqlqo.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gsmysremc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gdzkwirvf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gxcprnzer.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpcelqgff.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gwjesmklh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghlfpremn.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gdhacpbsd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gbaxihhgi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gsdejcobu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gospbzhms.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gvohdnajc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gmvcakwdf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gmhnbhtqh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/glaacjaxs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/ghqabfcvb.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gebupgteu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/grtnxiaov.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gnlxorihl.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gfdlzyjip.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gqhcmoolf.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gnzlvjkdm.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gpcedukvw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gepedftkn.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gcdpaumsy.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gjzmiixlf.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gzeuiizuu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gjiqvpkfw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gxwhyoapu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/ghnlhljfj.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gkqtophhe.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/gwqeptxdz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gruysboef.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gjaypclvi.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gglqxpwqw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/ggkdqpmjj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/guawitfmb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/glizbcdic.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gzmaapcoy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gpaywfnka.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gfxzhzsbl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gmrvtjosy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gpdlsdfph.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gzundudyk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gnfccuawo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gkmnflvql.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/glirlgcit.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gmhblmuek.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gocqyujpc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gvoixfgmx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gltmbmizh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/grxbjuugd.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/ggmzupwrx.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/glprztvbm.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gmzrwrwls.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gqcuqvrbl.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gcoeoxtqv.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/ghiyhccgb.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gossqablb.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gdtkembsz.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gxovzqxtd.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gxsrzajbs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gudbpwapy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gwiaubqak.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gaaabrxwq.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gfsuvjmaw.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/glrwrzlzq.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/ggznzusxf.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gbauefwqs.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gclwanlwi.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gwcnoesco.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gencfjmhf.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/giebdtkpu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gueoqpzps.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gigfgcdbu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gzehmfude.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gcsrdkdhz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gssffmoai.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gjjiptfia.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gfawquqja.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gvngtwmsh.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/ggsxjsxfu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gspkukixp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gicyyoazj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gwlneuhpn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gwsjirtob.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/giavgvilf.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gdejerduk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gytmbifbm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gbcucmvwk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/ghazlxiwq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gvsjmcnyx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gagouybcp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gihutonbg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/govajkeqx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gmkbbxfef.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gyygruckx.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gmkvcevva.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gyfmdiepn.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gxfpgocde.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gtsyxxdum.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gehdlphle.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gbodedyqd.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/godtdcrlm.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gayybnyux.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gqlfnlyei.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gibqbxxsu.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gmycgzsye.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gugugferh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gwrmgahcq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gpylzhmgl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gifookoui.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/glnvsoucr.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gznzuqqxn.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gulddfynh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gdfjprata.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gotksnrer.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gyuaoqvdt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gdhmxmuim.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gmgekvwik.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gasmrykkz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gsfkcaoni.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gafvgydoy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gqfknjtpr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gwdwrievy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gkyjcxpkn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gmyqtkhrq.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gmbqwwrue.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gedsnwndi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gvzsdwelf.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gbjjmintu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/gugjthmic.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/goxjvbgke.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gpcjnhewo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/ghuamkwhn.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gvpsefzcg.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gjtvdncln.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gmmknhnic.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gqsmrseju.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/ggjdwhkiu.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gvydzrgjp.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/giwmyxazz.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gnsykmoww.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gbxkflftt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gyrhpewpe.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gtgclxcwg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gmcxztzsg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gbvcxponc.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gjbevaffs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gydlimbme.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gthksunzs.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gdnzjttzv.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/ggtreattq.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gnyhmwdny.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gyrixjpzi.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gkglfughm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gwucjcrro.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/giboqdbth.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/geyxfsjxc.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/giqlopjvl.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gvndyzzae.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gabgcgiuh.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gbifwtncp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/gqgkzpnox.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gvdrtryvq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gqqcwbvff.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gebynrcyl.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gyyauedoi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/ghtisvszq.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gagkzincz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gfgbfqgom.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gktaaicvm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gypcbqnwa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gygitbjhw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gljbhiijl.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gfeuumiii.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gfcbsxhvq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gjlicgkqo.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/ggpiwvqnf.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ggpiabamj.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gyxzocwqz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gxcslhmzj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/guyouheaj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/ghaapsloc.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gcjynvwmp.sHtML


<!-- 参考信息 -->