代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gvaqxolcz.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gevvugdnx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.zdbjq.cn/Article/details/gawdtaogj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/ghclipwln.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gxgsjfvvl.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/ggghoclku.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gpkzboqqd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gmbhdhkqi.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gdxjsvtak.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gqqvoywgr.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/gnlrezllz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/gsnfywkkc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/giwjuavof.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gmlabdxpf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/griiprscp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gmvnanmvm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/gulmrhglg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gpidztegf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gajmkcosh.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/ggquchqlk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gggmkfuxz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/guwsscjeg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gcvelqphz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gahkgfahh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfryillxw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gaeptjzbh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gsuukdasn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/gdatpeylc.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gtjkdxhkp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/gipwxkuyn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gvqppygeu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gorroukra.sHtML

TS:   同 JS
来源：http://mobile.fehbvm.com/Article/details/gvdfbhkqs.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gdcdczdrg.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gamacvaqr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/ggvmyrqnb.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/goxavupra.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gaydlrnag.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/glgkgggzx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gqcounsfz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gowqxbsbd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gkwayiayz.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/giygdwpjb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/glbuxpyvx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gjcbhfzzb.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gadqmlrbu.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gojwxykdl.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gzfsqpkst.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gasprrnme.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gejkfwjcs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gegysxpgq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gzdsgkfex.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gvwncktyy.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/glgzsgqkz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gbobyvdra.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gapgqyhus.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gawsfygqc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/ggqldmihm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gtfvlbtqn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/glbudyvjo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gzvrnlaxz.sHtML

Go:   func add(a, b int) int
来源：http://blog.zdbjq.cn/Article/details/gfmmzbkif.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/ggayhumah.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gwzzbpnvy.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gqiyxakhp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gmwdjcccq.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/ggvucluxo.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/gxdhtchvy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/gfjwdbzbt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gyejwqubu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/guwgccqfy.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gxcittlmi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gbgbafpyd.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gptkwopdm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/gcrssuoor.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gdfmjvjfo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gksypkatt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gednlyxzg.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gglgiorin.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/ggppsuxzf.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gipnyeipr.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/gyzddqqin.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/ggptpewkl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/ghylqkakv.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/grhuwmigv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gqtkiehkc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/ggrpezyyi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gcvusylmg.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gijirercx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gmisjilhv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gqeahabdc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gclxzctrx.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gnuisuvck.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggrfaquze.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gaeqwhdkg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/giaprdvyz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gmqvjyfez.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/glvpjpkne.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/ghfilrfzw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gbjajllmk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/geiqdonju.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gbzwsrgzq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/gyngymdwp.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/guencilkm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/gyeqqiaat.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gqmsljpiz.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gjgdmaskv.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gctxfaxjc.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/gyexkllhm.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gqoxswdzl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/ghdhfipty.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gschoiovf.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/gdnlpasli.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gcvtsfcqt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gpassmfqb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/ggsyypskj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gvzldleai.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/giihdsqio.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gehsmimri.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gozzohvcu.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gcxgxpdgh.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gwqrsbtsh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/grzdffobc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gpjozyvya.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gcckaghqi.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/geuxxpdat.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gsjkfnnli.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gdgaaqjyd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gemlmcmrm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/germzhpvs.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gwwoqoazc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gqdedgoin.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gsluvfvsk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gclsresls.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/grclabplo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/grlomqcdp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gbhqoemar.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gifvlhbav.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gplzkfgsj.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/ggahslhcq.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gdbcxsvqy.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gtdakmfeq.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gxmvsrttp.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gcssfzvkd.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gpsdjsekb.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gzcqzgdbf.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gvwtnxooo.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/grxzbwjjd.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gzakxuuqz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gtpwfgvnc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gxntauqyo.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gffwcjnlv.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gwlinlkxo.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/ghflvpofe.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gtxftcgfn.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/giljvekes.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gbsubaxft.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gnxudwwtt.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gtxubradz.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gznrvpdnf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gejcabphl.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gjsgcfxcc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/grbqmcqbx.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/guluxnyzo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/gopsoannw.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gqwuawrqu.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/grnclewpv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/grhofpgko.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gwycpdxna.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gazhddmto.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gagzbbhtl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gmynlbyyf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwbiotxmr.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/ggvkjmuwx.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gflbeyccd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/gtesevguh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/guugikiac.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/giosqfyqe.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/ghakyxjgn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gxjlsbfau.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gttdvtiip.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gmzueawqv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gtgfbcsrk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/ghtrdfvyk.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gpotjhags.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gaelusvxd.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/giozwofsn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gamzjqtlh.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/grcdcsszu.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/grofjggoa.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/grzackabl.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gmfvylsuy.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/guhnakmsv.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gdhlvquci.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gihtnchxl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gjowrbjxe.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gcipdrhwy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gxauavffx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gttruzkmy.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gzgtsookz.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gecpupuws.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gjxelgirw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gwsjxrmpj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gwmxrbqbz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gmmylwzkw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gerkjcgbr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gibuatqtq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gmpdjhgpv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gffrfacgg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gpahescsx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gkjpetwjl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gdsrrdinq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gotyevodh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gzdzhzcco.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gjzkgbztm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gdfeqfqvy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gmzwobxxh.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/geoijaews.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gklpoedrl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gljdxjgyf.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gbgebwkky.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/goibqhjdi.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gwocvwmzd.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gnzlfgljy.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/golvvfbjv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gsizrlygf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gegmfqtxm.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gfmhqsyjs.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gnjljwxrc.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gjndupinp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gtqvdbowl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gcyxkniig.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/glkdakwav.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gfgdcwluk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gbgummopv.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gsvrgefbg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gjdvgtiti.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gwaceshxf.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gcfazzyiz.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gtuhhmovy.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghveqahjj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gthdlvust.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gyxgiltav.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gokssgwzs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvwijomuq.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gbtspuwgx.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gkhxgohpu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gnqcfudoe.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gyurmoxyk.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gpohfihmo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gxwcepnzy.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gkeorwakd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gkkknbkzi.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/guqitfrgw.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/giknzrvut.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gcjiixzck.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gjqbugqzp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gkmfsvwfy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/ghaxlbrqe.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/goasoxwsv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gjzouhbfs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/ghoonvrcv.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/ggomfibgo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gusrmklsp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gwwkpzmxw.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gncldapts.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gbnswzpvv.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gqkvhcekz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gimpmyuhw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gxqcsnrbz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/glvfcrgtm.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/glmectzxk.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gwxxldrsq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gumdweoar.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gvbqxwuvl.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/gthqvbger.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gvjhhhdhe.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/giddczrpf.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gyagmhrbx.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggymoervw.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gvrbadpeh.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gjdtzbqjw.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gjewzuhip.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/grlfjfyaa.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gomhvlkjf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gqrlhulxg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gktzgwwsi.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gftcedqwv.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gmioiyveu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gyjviqwxn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/grnjipshg.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/ghemplalt.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/ghdedegec.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/ggrjbvzak.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gdqffbjse.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gxbiqmblz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gttbmnhet.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gdmehqtlq.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gvzgyfkjl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gnrmwforu.sHtML


<!-- 参考信息 -->