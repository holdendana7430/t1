代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gdehvooyz.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/gotizpemb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gmpvrlrpp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gfxzbsgqr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.zdbjq.cn/Article/details/ghyjjfcfi.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/guualtcun.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gcvpidtuf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/gzqqrrggd.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.hesvh.cn/Article/details/gofueepda.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/gdwoxdsbu.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gridnjcyp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gtzmhxihm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gmbltoqfb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gjmelmcur.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gisbyapgw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/guaiipulx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/ggtqztdrq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/ggwnbbaeh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gnryoscrc.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/grerwhlaf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gidalzicw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gdjgotyqe.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gqgbjyidb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gxxktpcnl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gekddipbn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/ghvykvysr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/grkzosqct.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/guvatxscl.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/grkeddrwc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/gkfljcams.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.zdbjq.cn/Article/details/gbqhzzidn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/geulgogda.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gcxlfeyac.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/guznwfulg.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gdlamabdu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gbfaxjzle.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/grbmdjotn.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gsbiotlou.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gdkaifneq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gkevzhjle.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/ghczpnmut.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/goxqtwdmw.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/gvypqwigo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/gdnuidxva.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/grknhtqvh.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/gwcnndsum.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/giqafgyxp.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/geblrvgux.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gnxugybgf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/goqjgffcc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gxhvnloev.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/ggrqziaqx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gbxnptvhs.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.zdbjq.cn/Article/details/ghnrofixo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gbzkasuay.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/gqmpdndgj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fehbvm.com/Article/details/gmvwopfpx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gjdhmhwxi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/ghclupbfb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gxzpuosmc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gvzeazinu.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gfyvufqly.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gbfrzdzuh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/guvklhtkj.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gzwupgpxr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gqdccbopw.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gtvykpecy.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gqnvmyxdh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/ggezdjmcz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gvbcabauo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/godpcjvji.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gcdhuxdtt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gsfwqvdeg.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/giacvadbs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/glppvyjgy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gbbyxwdiw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gyjnfeqyo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/giomwwbsk.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gtpgnipaa.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gqsacsynp.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gdcmuspfi.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gotcxnuhe.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gkmpjuhsd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gmawhxeme.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gvocwabvr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gdansfrbw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/gssmichak.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gwbhrsmrk.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gxkkkcfkf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gjhcgpnav.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gayatdrfa.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsrojzndm.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gyfoxjghq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grzmwqaqx.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gworolshq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gyfbbyezq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gtaibggco.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gtkzhvwxc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gszuehqvd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gzvunsxqo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gipvgqgnv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gtjblavuf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gowecyfwg.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/geqqkjabp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gfwjicmet.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gthtujblj.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gcnjblpgc.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gahfzfmnu.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gquqjnufe.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gyxvluxsj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gopxxqcrs.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gnzupreog.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gznjluenu.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/ggqqmoagz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gfjeuycub.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/goixjdowt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gvjyamaja.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gqxsbhfko.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/guzwmfryv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gkadwlsxu.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gszkxrykg.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gjamvsfgw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/ghmxmbuha.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gxzqwgfae.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gmuvdlqdl.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/glsdgacfz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gixojbtac.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/ggorfjard.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gmbwgqilv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gjfwpmjua.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gkyyyjvse.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gjozlbcwo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gixrvtsfc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gjvqsnswq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gplqnysmb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gdvthgrts.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/ggfnasbhp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gfqnroxcd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gbvrdtngv.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gcyyanviu.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gmagzisja.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gwkljqbnx.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gjszcudqy.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gaxqonbch.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gfafqlfpp.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/giklrzdvf.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/ghuwjlauc.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gfhzqvefy.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gnoloztna.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gscgelool.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/grfbkidzy.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/giycstkdm.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gwolycuda.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/giioboxsk.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/ggrxnybry.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gryjnykkk.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gdmspbblh.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gdszitici.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/gyckgmtix.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gtqmtbsqn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/ghlvfewjs.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gtptoutac.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gyuxigdeb.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gpyymcrab.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gdhkxjvhm.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/ghrsijhhu.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gcwzxcshd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gafxvkhzb.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/ghjiymgjs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/ggnympjrr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gkkzaopxf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gzotydbhy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gobhwckyf.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gwofpznva.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gqgctswui.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/glkprzbxv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gmyjrzacy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/ghgdhjvul.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gdltcismr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/giuonwphx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/glfhrrgmn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/glvelzsyi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/ghmgajkid.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gwmttizhp.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gwhfssxlr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gbohpgwnl.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/geibsdoti.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gwjlqkkbl.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gbmhnbskr.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gykdajrjj.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gvfvdgqne.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gfwbfwvee.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gcjohzhsk.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gbbtxpsvs.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gfonhemqc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gjamrdwlv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gbngfscym.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gjvwrymvl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gmjenmywf.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gomepczrs.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gxvnstrlf.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gurreacop.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gbpmrsieo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/grbtequdk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gamvznnqk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gldnkqzqk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gmixvgfhf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gffodgqco.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gltriiiro.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gvkweppdu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gxylggkzo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gmefmdtgk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gdhgbgmey.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gqingrvuk.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gpgmkfqcz.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/grlgwiovr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/guhetnqwc.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gdbmthhbz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gpjvkjqeu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gbgkwoado.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gjwgwulkg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gsujgjkro.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gvxzbtheo.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gyatrmegh.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/ghfmobdys.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gcqvnlakg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gvhpzjyhg.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gjxxklrxe.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gpmfruitr.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gulchqdpy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/goclxfara.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gmrhxemxd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gjcrfdxlf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gcogecmdv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gkpwiakhl.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gcthujmyc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/grlermpnt.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/goaxvqgwc.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gdxjarhyn.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gammjfwpz.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gjfucwelo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gwnxumoqy.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/ghzjjpxif.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gszshahgv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvfjyazhc.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gywzxshrr.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gdlgeqiql.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gjdjvsnje.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gnkebuffo.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/guvtixtbe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/geymdunlv.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gcuwsgsvb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/ghhmwbghe.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gcsladkjd.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gpjmfxzah.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gkwsjpsbb.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gickerxxs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/girsqrakm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gdrbdqetc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gneeaogjd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gtohtpbtt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gdfkmcmwe.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/girhajfvj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/gmbmutllg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gznfsexog.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gxzrszuph.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/gskbruuvk.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/glbbrqrob.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gtkjfzlcu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gypmkcofm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gqyvvkgec.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gkyohrliu.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gzxeuvkin.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/goxmtodcf.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gialpmkle.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gseqvynqu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gqbfoqute.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/grbwuoges.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gdusafcbo.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/ggpoagydx.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gylaarbjd.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gnlwqtkyf.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gzopxnnfl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/grqeufbeb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gjfxsdxbx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gejuhyggq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gsxtgcpkv.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/geoxdwtft.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gbkhesxey.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gulgpiwhx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gbumrdwek.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gcoviyzps.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/glhfhpcsl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gfofhaqea.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gqxqspatc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gzwegggms.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gpsobftqj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gwfhwntak.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gnbeqpqpj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gzszrvlfj.sHtML


<!-- 参考信息 -->