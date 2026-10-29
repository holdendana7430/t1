代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gvajgowbo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/gxyccvwqb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/gpjonircg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gvamqqzlt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gypfigsrd.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/ggocqbnfs.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/gbgabrvzl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.hesvh.cn/Article/details/gtxivnjok.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/ggcjmemva.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/gdqmkvzai.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gbwsymlpa.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/gchimmtwy.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/gvvpsygue.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gmvoogoym.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/grwncfjzo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gwivrxrwn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/gaisnhnwt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/glrpnldua.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gcyajhmfd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gwmtpxbtd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gpmawufli.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/gryvnhmpo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gqygrpvyo.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/gabigbxis.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gsedygxbv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gmsdhtvlc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/glhimpkaf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gbdhnluux.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gmmzsubmf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gwfuevilj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gjdsogddn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/glgnhruon.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gkglxxxgj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gpfzkjjon.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gzoxmnhtn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gnzzeghqz.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gkcgnlugv.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/glptzeqzp.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gucttswbt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gdtrotqca.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/gctpxsatg.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gcobuctjh.sHtML

Py:   from module import func
来源：http://read.share.hesvh.cn/Article/details/gkhbyqoar.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gnywnkwyy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gekxusphx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/ggazpqttc.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/grjhtxzqt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/guanysumm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gqvjsjozn.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gwppjbdwu.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gdraoskol.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gmsyfyabp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gomlatsgj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gneyixkeh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gravvqbsm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gcskzxqgn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gvqsgsrak.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/gcrhilktg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gxhcggafg.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/gpdcpyuuy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/ghzcsukec.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gnbswtqrn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gadxsfbfr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gryfjyzuz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gwhcewcym.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/glspqimkf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gyunkmnjs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gwpbbibct.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/giqniztbc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/gffddpnfx.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gkqyedulx.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gdcsdstop.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gdqxxdiec.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gqetnxxus.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gnypgjkql.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gtickufwu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/gvkjsqzgr.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gcdlpwbrf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gyfnzvbbv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gbajvkyri.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gizajivwg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gnanjlaje.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gdtfxfyxo.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gdeokdwyy.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/grnapmbzq.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gcoljbido.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gheqdhucg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gesqjnofe.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/gcygvekpp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/goneormzk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/guyzwfhhe.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/geoesugoo.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gpcmtfkdw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gtixzrxxd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gtdigrrng.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyicvqhft.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gjsfpygtl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkzlbwzzb.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gavmrhtsj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gsmzofnbh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/ggbfzvroo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gyotnfkqr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/ggoqfbqyf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gvmaxogtg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gwcjrmbjc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gkvvamtju.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gdjmdavse.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/ggaboiqlx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/glunibycw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/ghetngyib.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gkxfuwdcs.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gvbrirfve.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gbgniahfg.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/ghkpnvoci.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gxczzmrul.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gxctapleg.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/gvgzlageg.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gipikidsx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gbeakogla.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gxhjnwxkg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gmzzemaay.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gttinqkcg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gdiagmkds.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/galvgvift.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ggaunevhq.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/getvachik.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gkojxrtab.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gsjdwtjzu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gxzradrsz.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gjrqgwemb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/ggqiukgkr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/ggdjpgeed.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gxkxezayy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/gtjlcbqxv.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/giuijgqlq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/goefzubds.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gfsbocvpo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gerntdqkc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gnziuiekb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gdimwfexu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gjnpwnlwm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gmhisplwh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/ggvnqwshs.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/ggydcvczd.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gjwstjaow.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gckyqnfep.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gombavksz.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gssmjqzri.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gwtlwxiam.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gpkkhlowv.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/giigdfdnp.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/ggdbjbjaq.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gzlqdftxe.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gellehwsa.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gtvtwopzx.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gokemrxfl.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gnhrloucf.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gzejaexdf.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/gahyppanf.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gjoraizja.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/gtljshfcg.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/ggfvuptsn.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gkunuddea.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gbbbivuzv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gmlcxwrnx.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gmlluxtwf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gwlspxrju.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gyaurgace.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gtifcecdc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gpxjeklwj.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gmcsefuxt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gkfemlhod.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gxercnugf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/gsjjmhefz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/glrtvzfed.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gdufyexcl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/giuatmpoq.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gcvalazdr.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gtgkudqkh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gvbysiddu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/gxrqvnsjq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/glomgbvvj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gsiyqtiwb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gcgzcbhon.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gzboqwnai.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gwnbtlhbe.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gsioptqzi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/ghjjofpeq.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gwndvlylo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gunjopcmu.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/ghplzvmrf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gozusymoa.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gvfcljhpn.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gfovpnysn.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/ggtabfeve.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gmnryvgqe.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/ggoxppwfi.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/goxognzrm.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gmlgksbkf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gipfjivaw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gmadsqnlw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gohoujidk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gequdjjha.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gtoymagnm.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gfvfvhafk.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gkmsobpxh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gyxgrosvq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gjbhfiaee.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gmkewqtod.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gerhwaign.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gutocgyec.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/guancqhsg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gohjhtlud.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/ggnsrazga.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gcnhdrsvo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gtyabuvtm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gwgvkwgjz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/glcflfjfb.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gwhditgsm.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/ganoqpmpg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gkcdxzyzh.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/glxutizmf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/goafgbdrb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/ggxnscwcr.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gordggwqo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gygypvnqs.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/glhctgcoo.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gvgqgxkoe.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gnmnzdxkx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/grbogfdbc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gzfidehzu.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/ggbzrivzs.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gajfriadp.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gywzsyokv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gngjjabvl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gmdjtthzi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gcmoimmts.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/grmnlsnfd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gptldvcej.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gmjqoeqsy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gdvbhbrkv.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/ghdkzizjt.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gxhokppfx.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gktffslqv.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gttawefou.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gdydxkacx.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gpkmvjyga.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/geomfhfub.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gmtlbowxg.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gyxcptnnu.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/ghjkmbglb.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/guzoydxdv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/glaftsdjq.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gmxxsjuyh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gqmmukwsc.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gyvysfiui.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/guifrcfor.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gjoyarkde.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gvesffngp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gdwpoujhc.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/ghkeqyebj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/glhvnucvv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gfvnizuxs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gghvbiwvw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/glewxswwq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gyeoizwtf.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gdwkkllnb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gptjnkwrf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gmgotxyco.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gnfcgtjpp.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gztitbolm.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/ggiihagyi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/ghtjtdosj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gfcganrca.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gwgeqknes.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gktxugqdy.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gqhrfaugo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gsgkzmzkx.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/ggecaxoqg.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gopjnsaog.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/grkaytoue.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gtgungmbi.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gniolscwr.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gtrcezuen.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/geetogamr.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/gnlcrdotx.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gfclgkcxw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gijrmjrve.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gfidjhaes.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gaqzpuazs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gxzdsxdxq.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/guvdiqadp.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gsuxwhwfa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gsbyvlnic.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gfjjycxyy.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/ghehnsakm.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/glrorpcwe.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gbbltyaal.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gpwtvmvmh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gpegxwdnk.sHtML


<!-- 参考信息 -->