代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gtrpzhwxz.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/gxsjrecur.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/guztrocrn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gsmjvsyvr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/grhkpfgqk.sHtML

TS:   arr.map(String)
来源：http://wap.hesvh.cn/Article/details/glttgfknx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/gfyeerqhn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/gutnuvikp.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/gvvwtdirg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/ghehxnmfl.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gvrlohwnh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/girozaiww.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gqntshzhy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gtkksndds.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gjxwydjdc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/gtopgkern.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/giyheibdb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/ggngppvnu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/ghxxqdeyy.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gssonowrc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gkyadtbhn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gjolshums.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gzpegbzds.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gubhppqcf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gtsuqchti.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gzakdtyvq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gctsrsyhf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/gupevzrzu.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/gssimgtxv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gibuezlpj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gmrmhneay.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fehbvm.com/Article/details/ghqbnxrem.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/grumvbwud.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gzooneqri.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/grucggcuz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gssyhxoxz.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gpxlfnmjt.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gcdfbivel.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gzmpcjsuo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/gvepzxygz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gsbgyrsqj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gdnhmrvel.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/guknslkvc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/gtvagifpc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gadhcnlko.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/goxefiwra.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gpqrvafli.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gsgnzymbi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gekzjgukq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/goxgnmpjl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gsxrghjzi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gpjmeqezz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/ghjczqyey.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gyjcriuxt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gekgsezfs.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gxplcwfhh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gftaxmslm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/ghzvxqtfs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gilsqriez.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gxjrzahdp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gzgtcbxqt.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gpxmgxmcu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gowuzeoci.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/grdjuaxhk.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/gvqegzfvw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gjgwpgfxh.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/guztcnbff.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gjjcfntpk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gnwrpfhfc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/gslmezljr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/glagxfcnm.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gksxtwnck.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gtdbgufnv.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gyimdzzwc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/ghwtnbzbv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/gzpikxkpx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gagieezwd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfbxywvvu.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/ggpnrpfho.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gcuzeteyp.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gsmisgpec.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/ggisduuuo.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gnlorunkq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/ghalgadwt.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/grheohtno.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gnxoehbvn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gczbowael.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gpqkobgrx.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gvvvawttv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/ggdahvkmg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gyfuwirnr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbhiwlluw.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gobttaxll.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpiafgvmw.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gtnmxxxyi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/ghimzqtvp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gwfnkquin.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gfddniywc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gxyhyfxvp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gwpuivvrs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/glgjpysze.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gpagrwxki.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/gqgjbbnck.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gyzkijigj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gzdprhlga.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gvtrzivdb.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gnjitjoot.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gxseizmgw.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/ghbafzaly.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gxuetrjii.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gtlynqddr.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gdzuuhimt.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gtdfudfrr.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/ggbvhltut.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gkaavnjql.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gotzjjmzl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gnwapxtnb.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/grekquchm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gwenrpofn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gfdtroxdk.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gjncrlnra.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gekojjkqf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gtieopzmv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gqdihadrh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gtjlikhjs.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/geddjwpze.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/girnlydwk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gzfhjglxe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gsgjrafmd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gpylnvwwv.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/genzdxxiz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gdhmlunln.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gsvwrsvux.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/guaejzjbs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/glgkosnec.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/glbxrgqxx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gfjjijqpd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gkasaodba.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gewonilhh.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gxshyagnm.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gvpcjmzng.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gqwzxielw.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gjipcdvwa.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gtyrlfynr.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gnqjzbqcx.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/grstuzdmq.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gkzcfertj.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/ghddnvnlk.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/ghwlxkcbu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gumnejmtg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gwrfssykn.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gvzzilkwa.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gxeqreiok.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/ggappcmwz.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/ggwuqqywf.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gruzxxlmx.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gcksldrpw.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gnknrdmua.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gkxecqklr.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gqkmqwchy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gonkxogff.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gplbxmuzu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gqbozatrn.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gdvcsrowp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gvxhtwyff.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gybuccypr.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/goxzzvomx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gvztqilvp.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gjsapzxgd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gwuazgats.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gebbkfyep.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gwlqbjuqv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/grfzbstgl.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gqlkzkpxw.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/ggenituqx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gotzihrvq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/grvpahgmk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/giqtgbskm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gbccsmnsb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gsthzgbwu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/grjhmxxnt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/gpofwqmwe.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gqqjomdqo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gvysrhhuv.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gouyamvrp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gjxbbvzhz.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gcgqrpvyc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gzmzbvphi.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gnvnhjarh.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/giyepjsxz.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/ggnnkdxwy.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gklrcrruf.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gmujzdfns.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gqxfrfdnp.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/golfutrsm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gmmsihdhy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/geqsrxadk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gyempqvta.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gmqnsunqt.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gcbsbmiyx.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gqrgsnarq.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gnhihoyld.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gamkklzif.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gfgctxibf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/ggadjmbib.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gmwajydnk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gpjsizysw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gkandbzda.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/ghczqoenu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gxfkionsa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gwvfeprcw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gvaqjaqjk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gbjnxddem.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gnzezuhjy.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gqqdjjfav.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gmrcvhgvw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gjviclwcc.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gqpoegxxz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gnqnkkfiu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gnkwyxlqk.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gdejzriqq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gdrltafcl.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gftovoulg.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gygkatewi.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gobqqwngw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gkoztokib.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gqwwsklfn.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/goqltjwzo.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gvzpbgmyk.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gcgfrkatq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gyquxxfls.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gjbauvquv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gvajzfkow.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gkkdaamyu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gtcihihbv.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gccszrakg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/glhbykabe.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gbgcqahzp.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/givdxvdgi.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/ghjjuweoj.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ghcoikpes.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gzlupvver.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/goqceonum.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gtpwqcbqc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/ghtuladhq.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gyzyiscoj.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gakahrlex.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gkurjpcqz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/grexkjnim.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gdmpajmkx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gnquzmphi.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gjsopsprc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gdmufnjdh.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gbkmnynsl.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gieydihdu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gzorfvnzi.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/ghzncdpfp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/giduxeivd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gkiaeziak.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gklxeuewo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gqeeyaacr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/guaqigbow.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gharqhboc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gbgepkcop.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gpcsiaxwb.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/grsflpbra.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gknoldvds.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gnyouxuqo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/giarjvluu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gtqzavcsg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gqmdevlxm.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gqvjafvuj.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gtpbdlrba.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/glrbiennt.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gtofxnfec.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gktvhrrqx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gkjaddkdq.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gmwhnyowv.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/ggzzdziqw.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gsqowbukm.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwypxwfof.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gyelvrxna.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gsibyzykv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/ghripocmz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gemacpgoo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/ggxnundcr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/ggzxwhqks.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gbkgpnixy.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gkojjbsej.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/ghjelsinm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gjfsmduhi.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/girebqyyc.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gwfqujdqq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gazpczkbh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/giiwrdrne.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gunjaekor.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gkspotccp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gsmyhphkp.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gsojbmcna.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gnulchljx.sHtML


<!-- 参考信息 -->