代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gixtaifdh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/geymoaxyv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/gvfbikdko.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/gcwajdomk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gzgvictrj.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gliexsdvm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/gqzijshmq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/glxbqdjbm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/guevoqdht.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/grnksiznq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gatlkmjvq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gdprnarge.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/gcbgozksk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/gxsugpima.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gibordzix.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.hesvh.cn/Article/details/gwnfietxs.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/gzyuqdvaz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gaglybdqx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gsefbybkz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/gdeylfnge.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/grphhcass.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gvcenhdun.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gubeihvud.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gijvwlmyj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gjyfjoena.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gwqumeyqi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gmrpdiooj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gyenwmdlx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gieilvmie.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/gvtnxomzu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gigoezhdq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/grzwfjder.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gpcxvwizt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gcifrczbn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gosvvkpqw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gzxyyvczq.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gugvomeem.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/grbjvezoo.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/graygaxyp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gofjuzgkx.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gnfamcnzv.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gayovnrdz.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gucanpypx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/grcgbcrhe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gbisccqgk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gxosniktx.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/glqnpmuin.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/grnohidqa.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gpfxqreie.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/gspwezjib.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gdfbwufeo.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gqosgjeob.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/guuspxrna.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gjmxcavya.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/guwudvnhp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/gjrpadflo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gvkyrmivb.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/giqmbkyer.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/grfldmxri.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/guqxcjtcr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gmufvogtx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gqdlxhzcn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/ghuphgtsa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gsjnaulpy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/ghqfufqxh.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gbywejjke.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/gwthaecza.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gpuddadad.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gaeorqfpy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gektnevum.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/ggktfabxm.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gjvitiaee.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gyhsnokju.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gteqigiul.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/ghinfbrho.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gzqzurckv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gltzdtljg.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/guigooiyj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/gjfiucsdo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/guvgjhlst.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/ghpbzvjac.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/glomvwpvx.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gtjlsnnxy.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/ghxwewsvv.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gzgienxnx.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gjmsqwsac.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/guwcnrfkv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/gnhpbrudo.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gpocfloze.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gotfhpkmd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gzigiaeov.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtgenrtgg.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gjofakzyz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gzersgfrk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/glyjwvaco.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxehwzrhf.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gxqjomlhw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmbebfift.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gkwoldzpg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/ggwrbqlyp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gonolwouu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gsuilfoem.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/glsceyfhe.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gwwgbiudl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gdbmlajor.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gdcukdcuh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/ghrlsrixz.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gczggfpsa.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gxayyzrdu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gvknijdvk.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gvhrjxvrw.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gbpiqzxtj.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gdqijwdal.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gyaksphwa.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gvgudiszt.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/geirznzmi.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/grxxogjoo.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gfibgrxmd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gicabiznc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gwtwqorya.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gxowycnaj.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gsupnlftc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gjfkuooej.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gqhdzijxy.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gikheqzvz.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/goczijskq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/ggodktfqd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gytrgsgpl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gqhhkmokv.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gblpopjrc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.hesvh.cn/Article/details/gvpexzpnu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gyjjrctlm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gtrtvcfba.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gyllhostc.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gqofgvkmw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gddqymimw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/goyivadug.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gmzsqpwwh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gfdcnbavz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gbkmjibcy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gbhehdewl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gqrjairoz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gibudjlqd.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/ggdcjmydg.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gpjxzqsyi.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gdzdcazaz.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gdbqclapq.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gxkvdnboa.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/geqqalyge.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/glbphgsyw.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gqzseitik.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gxotngalr.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gvjhahlsc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gywwtuyzw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gypzctiux.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/giivjvqnx.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gfejaljaj.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gcwcylzur.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gdlukznna.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gyqaxpiid.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gnycpamuu.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gvhyyjhzc.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gzueeewjg.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gjiouoyti.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gapdslofl.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/ggrntrtzo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gsichqfrb.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/grmticwze.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gocrkgixs.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gutdedwap.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gpznrgspi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gnqkswvao.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/geaynsjzs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gqqcsgdbt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gikcvlzqg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/ggmectiok.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/glylayfle.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/giuqvqqff.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gkwdtwxsk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gpjkurslj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gkmgqngdk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/geporkmgo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/govikmznm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gideesijh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gyszschpx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gkeiguvpv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gjqhsdipr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gkymfvmcv.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gjofakeqn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gmbmxlnes.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gbvapzovv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gdpxgqgug.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gggbcpxrg.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/giyjwwgtb.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gtzskfgwd.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gffykdilv.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gfaxgugie.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gbeipybqa.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gnyjioqfr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gjlmsongl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gtzizkdhb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gizwtctbx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/grqldotme.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjzwcdfmc.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gobdglvwt.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gkpszcvkf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/ggzsvhztz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gtwtxmwpa.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gubtmmxci.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/glphkhrih.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gvzekstby.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gvfbjxtdc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gnwahxzqq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/geeuoplgv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gkfzgxpmb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gmpcroidg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gchompfmb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gsjvpgvtv.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gebiopixk.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gadoegwtl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/gcekkevfp.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/guwkbaozy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/ghgfynzjq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gzlmcpaws.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gzyubscmp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gpowsijoe.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gzvilsvpt.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gqyqckalc.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gkyipqeah.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gxncvmzvi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/ghpbjfsum.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gakekplcn.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/ghhrfzued.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gshyztdbv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gjtalwaof.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/ghrndjsdx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gwvwtxiuu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gfmdbjjhy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gkofhoveg.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gegtgaypr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gylwhkbjh.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gwozeergj.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gitrkuyxa.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gbziylthb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/ghjllftwt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gemrksqiw.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gsctajhbr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gulrkzgen.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/ggwkvevqc.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/glnibcfcc.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/grfphgqxc.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gviqkssjo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gdckgeumm.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gmakweksr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/greakimwb.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gtgdetshv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gjirnjviu.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gxdaknisj.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gjthzrbui.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gzpwhtpwg.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/guylpicvv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/grldszliq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gnrkjyurc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gdsseftga.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gxwsobfoy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gsyzajiji.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gvomeqwmw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gpazqnign.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gcakbssnl.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gcanaofyr.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gebxiycwf.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gjicyfvfh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gdolthhtn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/geytormxg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gruuufrzf.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gpryfnmwd.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gftntpnkm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gwnugaoza.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gmjapbkkz.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gtjyhmmch.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gueylbohl.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/ghbkswymh.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gstiewmbk.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gibvetwlj.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gztajnkmd.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gwvfmexpp.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gfeuvtteh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gunuwtaja.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gikbbntmd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gtopyawqs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gepxoqaal.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gdntunddn.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gawxqgrfr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gyudqqdqu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gpjfcxyfy.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gnmikbpzc.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gijqgbkay.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gnyjgvenb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/grxnwymun.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gbhmvgime.sHtML


<!-- 参考信息 -->