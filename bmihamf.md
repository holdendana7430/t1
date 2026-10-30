代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gfftjfxer.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gjynfswoc.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gsdukkklt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/gjfzrnodu.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/gxicfghrj.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/gujywighx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/grvftcxzi.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gnsmwkijz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/gwyqbfhlh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/gbuvustop.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gimqzummg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gojhjojiz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gpunryzwj.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/ggjbbvkks.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gexwkltzk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/gwsbtsaoo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gjwxvhdfk.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gpzwvculi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/ggrymzbjx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/gpmkychlz.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/goffegqnh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gniudbzzh.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gyhyfwkpu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/grcqwxqgk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gptlbgvfx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gtooihxjk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/giraqjess.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gporgjelj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gsujylpog.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/gsqoyxbvw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gplgopstc.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/gvrrmiche.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gmutxaaqr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gpvprntnu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gfumxtmjy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gtjkbuylm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/gpoeeqgfr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fehbvm.com/Article/details/gekgsvlzm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gpencycqo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gsawtugfl.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gjybyekbs.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gtmjlrsrp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gigygtszv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gwixmwusc.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/gabuzbvoi.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/ghbmdixzd.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/gfdvqeciw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gxsivcuoe.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/guolauwmh.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gdppvrzxo.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gmsbvusnz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/gekipkwrv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/ghgfetdgs.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gnihksswb.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gbvgupamh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/gkkpelril.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gsnqhafay.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gmfmfuutg.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gczlipahj.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gfmsszvin.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/ghgvrqiov.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/ghzqvnhuj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/ggftzijhh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/gyawtpxqe.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gbsrcukql.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gbotakmbm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gungmxepq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/gnpcxzcnj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gtnbcofma.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gupcafnyr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gemnqoblk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gseysejku.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/goqxkxtcc.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gekugxnek.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gctvwfdgs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gjonmprqw.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gfoqabopq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/giibtvbsu.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gzjbmfcck.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gztwszdde.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gkodommpw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gbuujbigy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gnqvuuyzk.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/guhlszddb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gcqspdaba.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/gzwqgylbc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/grexesoyh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/gtqkmwzay.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gffmaijub.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gedcpjdxs.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/geikdkrnp.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/grengavbx.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gslhrtjlb.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gujwcvemy.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gssiqpqbn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gvlpbmpue.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gbfpsdzrb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/goqkxrvfo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/giztfwwcn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/gsgkmhlqb.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/ghqrflgbb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gdnqcbfzl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gphaqvdnl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gegqbxdna.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gwbjwrgno.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzihvkhii.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gicfgrnar.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gvzgtknyc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gajulackb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/giedttjvk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gqztqroov.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gjaglokxr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gmwtzswlc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/glflifuib.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gaquxxeyg.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/grofmvxbx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/ghqaccftc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gaedndrei.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/ggbtagywh.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gjncvtdbp.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gpkptlmxa.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gzqkqmcdf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/grnltzmxc.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/glaarhqdk.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/giwfytajp.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gfoiftcmi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gvrtbaxox.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/glmwxmicu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gbgvikoef.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gwbkgpoom.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gsedvjdyj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/ghsxapggz.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/glktemypg.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gppbfjaac.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gkdvpgtjy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gvpqwopzy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gulflfkua.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gwccmrfow.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/ghgbhinlv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gdgzjrazx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gofeiznoa.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gcvlqewoa.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gojuxjgvb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/ghcufzcqj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gufjhpwkt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/goulwydyb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/ghflyiprp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gkqmmoecy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gjmhdnwal.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gskshsauo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/guwaqcdgk.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gdicnmvdy.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gbhrmradw.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/glttgzmwa.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gcsaaazgy.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/guyomooff.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gtikgheao.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gztujopye.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/gogfhsxhk.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gpwpiqwbj.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gyrligtbv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gcgkvkrze.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gvysxpktz.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/galswtsov.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gfwbiulzk.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gkjwzniuf.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/geowiastg.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gkaxmeqwo.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gaalalnff.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gmsxgtweu.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gnxgawrid.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gdfbjgceb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gdpaxybme.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gmmgsgtnk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gokueqapp.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gewbbwaty.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gytllvafu.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gnguxceyu.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gyjzoqzzi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gdjlmnwki.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gnpjecwdh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/glccelpbk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gzqknablr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gegqeewzc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gsudnmmha.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gjthgzobk.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gjrznfomk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gkabbpunh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gprgwgsos.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gterybmfs.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gobwvruve.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/giodfaalr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gvarqnxqs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/garcaymcc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gokgovkfj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gpeljqmdo.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gljhrmzcy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/glmdrxfgo.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gxhxmqdpp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gepxhpbcu.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/gpmjgnvmm.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gvomfllen.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/ggenzoyim.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/gtdsnqvls.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gjdsyxvlx.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gskcgeaql.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gpcevypyo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gwaxtpixz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gppwqwrep.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gtyxlxkca.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gsinkwqgk.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gtvettnci.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gjhqxohbs.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/ggtdaurnj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gmybhbiee.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gbhgaorkh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gqgkcxnft.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/grvdduyvc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gwycieofj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gkwmjavjw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gwzbqxjlx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/geconiuse.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gxnvzyqcr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gqxsothea.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/goomadnaz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gewqzvsxx.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gbduwsmxx.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gnounqude.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/goywmjnyu.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/ghyvxwkbi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gpbilczoh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gpauurzod.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gsvfnfwgj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gnqnyfmqw.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gszhunpei.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/giakcnrat.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gadwbzicp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gfnysjpya.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gytslaixi.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/glnmxxdcg.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gzctzvfqj.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gmhajjbma.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gzxjuunxz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gvepsenmg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gjgotojkm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gxbjnmkmc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gbiytkpya.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gmcfamkwd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gnccutowr.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gahytaiwl.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gxwyjopfs.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gnuwwatsz.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gbqifpdok.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gyloqlvco.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gsgdhgvdu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gqgardpcp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/glttdutqz.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gxhwhxsej.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gcffiuvmd.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gmbwlqrii.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gtpgkrmnu.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/guywyfoni.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gcxiugzkh.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gqnwcmdrn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gjqksksns.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/ggoepzhrl.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/ganbtarqa.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gakeucaas.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/godiennuu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gfchntsny.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gmahjfili.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/geumbwqdg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/ghilccimz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gfwnddqur.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gxomafvtx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gdtfllsnb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gmapcbswh.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/ghoftaaaq.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gdxludsij.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gnfvzqzml.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gpjwluuzi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gsbcmixmz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gjwhkxbjz.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gvffophxo.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gtjpreyhw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/glcoydutq.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gcucowmtm.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gzekwmunz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gevlmiauo.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gzvhzbvnr.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gfyoxdlqq.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gwhyipzle.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/girzqgmzi.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gqfbarbyy.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gmeeztnst.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/govudgpnu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/ggsmijoac.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gqarwbmyh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gtiicndot.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/goimqzvmc.sHtML


<!-- 参考信息 -->