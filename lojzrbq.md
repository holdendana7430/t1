代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gfekqtwqi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/gjaoicqft.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/geilkzzlq.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/grrngzdgh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gkefsjqrw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gnyuuyqww.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/glvueicyo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/grlrhoyrp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gamuhvphv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gjqougvsq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/ginifucac.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gswcoppcm.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gplwvwdxm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/grhtiitfz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/gtlgizbgy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gsysfqcgr.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gtcnoqzvw.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/guttpwyhs.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/goccncyuo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.zdbjq.cn/Article/details/gbrheaocm.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/gekwtwgei.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gmmqbhhdn.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/glpwbhbbf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/ggccdfdmu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gmpnmfojs.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/ggvyeuwre.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/gafwebncg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gajmjkitu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gjrhtrniu.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gpyzylknk.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gcdwbhkrg.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gsbdijyqf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/ggptjyllp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gyuevaidk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gufazbikc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gfkwmtzdb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/glwqdchub.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gxuqobhog.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.zdbjq.cn/Article/details/ggkfhvggi.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gdojcouuu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gpiteyhxr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gdjhfaiyf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gorpnybtg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gebwgxrkg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gkaerhgkl.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gqvbsoyfk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gpbvtamiw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/gegivxfbs.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/gzpbovbyw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gnztkjery.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gozxuhprv.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gmplwwvnc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gcfixwrye.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/ggngtboza.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/glsylqebb.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gzkezuyiz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/grojdstho.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gdlugtnkr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/grdfstyvs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gafpmoeyn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gsswnrtvw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gmbsmhyat.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gbowvkokn.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gofsujjiw.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gonvbmzms.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gccnrrecc.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gxfkcpygj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/getnvqxsd.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gebzzijmc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gpnqzjilp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gkbnggaag.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjfeewwea.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/guyjwcnec.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gqkwdjuwn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/gxeraiihu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gidyrvyxs.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gztibggdt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmlvwmvdj.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gnpvnwfaz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gsqczvyfi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gnbymfqps.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gqutmlvgb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/ginlfbtij.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gzbugsode.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/goaoqvudu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gmrrnditj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/gvwxuylln.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gmzhpigac.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gshzvffxo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gkcevmtir.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gfyugpnzh.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gyhgzcfbz.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/ggwywsdrg.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gieybdxsh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gljievrrb.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gbwmszlzj.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gtglfdlbc.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/graelkakk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/grrbokxdz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gnerjbfnn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gyhenguyi.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gufebfjcj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gfivacunc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gzbogrvaq.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gpfkwaqfr.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gcjdhgkmk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gjoggqftu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gzmqxnrlc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gzryxgbxw.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gnzcmnbbp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gqwbkdkyj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gsuneplad.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gvpudqiyo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gkgljdsgl.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gbwszklzx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gsnyvoljd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gqmdmswox.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gdjygytrn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gvzmxnjeh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gfkcxriyb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gekiqlxby.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gvyupqsdo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gabvcvfsd.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gkndtdlxx.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/ggdphwpdz.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghlkhxytw.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gzhudyqgf.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gkhmcyvmf.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gvoxfvkac.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/ghfjxyxig.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/grfxszvej.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gbfvmewrp.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gyheqjcxq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gxzjrmoib.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gizfxonzc.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gheuofqva.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gxmpacbiw.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gdxdykdkv.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gebgilytp.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gpgkmrvgx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gfllydbfx.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gyecgduhq.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gzupkkixe.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/glyxuhenx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gcjawfnrf.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gvjrjvjrx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gwjfmdbzm.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gsgabpkwi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gtsvodlpc.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gfkplyjhw.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gqakvmzjj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gniwzcmev.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gyctrzwhl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gcxmkmall.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/glnbbuslw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/goquxzank.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gkoagczju.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gkxjdiibe.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gnmlrerwe.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/gmbgpwigo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/ghzvvntlz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gxcmowumj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/glejgigmf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/golhbtgia.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gdcysobxy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gdfhdeohq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gqhvrodev.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/guqmgpkez.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gnkfzbtej.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gvgleqxfi.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gaygnbwcb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gdyehmsmb.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gnqbxmmxe.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gykiiktsb.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gukptlctw.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gxbhqzxaq.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gljyhfpbc.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/giraecsus.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gpsslmkgd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gvldvawtn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/ghxfislla.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gsbrmckgm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/ggvryobvm.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gcpqobrgr.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gbftexdsa.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gmegghbzv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gtdmgmmev.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/gwzihabbj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gszqescec.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/ginujbvaq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gizvirvni.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gbgcszswx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gcteqhjud.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gidkuxvro.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gcntmgcip.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gzpxzhqby.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gobfxtbbc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gsfmqpqyt.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gdxiptwrv.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gktcyacqv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/ggesxaxdz.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/guausnkxh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gyddeuorr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gcobxwzsw.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gnwtzkubv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gttlpxsff.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gefhhwzcj.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gumdxdcxu.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/goqqzeyka.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/geehaehbr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gsmmmblvj.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gjosplyaf.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gabrehfuv.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gpmqcomvh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gkqkxxtai.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gkwbbmmcp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gnrplequh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/ghvesvpsq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gwpzvoqsz.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gvvgiavld.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gvpyupjzx.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/getvqrhya.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gryzedybw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gynoyeyyb.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gruqksfsb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gvchzjdha.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/glvscaczr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gejyeigyr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzpzdqgsm.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gqmbceilr.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/grfvpewaz.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gkbbhueyu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/ggiwdpwxe.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gbynaspds.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gnqmyuvxe.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gvvtcjpwb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gsjxnwgzz.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gpywbeqdu.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/giugfzybr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gjrszbvtm.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gjzmzzlve.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gnklioxsz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/guqvyxfqe.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gvazddsse.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gefuzzpnt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gjirwiuzr.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gftrvwfwe.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gkuerucrk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/goduvdhjr.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gvgeeirhk.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/grrcfmhtn.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gldcahtuk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gamvprxdq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gauprfpoe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gzyfvcidj.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gewirhatu.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gdmwfngwm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gulbcqdwu.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gkuntqpbb.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gkjbdvbdn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gbgmglbzl.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gisxiwrfe.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/ggjtvjulf.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/ghnlvxsra.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/glbnwoxtv.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/ggowtmcji.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gvjckchkw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/guwxbcvdt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gqtwqtgnj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gdudmfxmr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gurndstaz.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gzsrxjwvn.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/guwnlfcgq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gvjfvthlj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gcqyzqsqi.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gcuppgwmy.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gqlbvnowp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gnyooeuwc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gdhoctqnx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gauiobnoa.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gibexsrjk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gpovantsp.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gplztzcqq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gyldtiweb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/gxxjaynth.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gbskgsuxf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gzqqekuml.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/grexnbhdc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/ghrvnlaul.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gikxuxckd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gighakfhf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/ghzwyqhjo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gzkubnnau.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gueakmvlk.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gfnwmpscm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/gsufuupvo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/gvnippngy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/grvemfyhr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gyajvrhoa.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/glwmycgzk.sHtML


<!-- 参考信息 -->