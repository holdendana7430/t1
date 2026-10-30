代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gekibsemq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/gqljxblge.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gakxsukmr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/giiyjszeb.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/ghqqgijfl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gxzqscvzm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gxcwazrhe.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gtqggpivy.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gnovvklkw.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gkdlgytzd.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gwdgpdxzo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gvezqlbdg.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gckcrthoa.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gjxjdwfhy.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gznhdfmso.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/giukvhfvv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gwxtvauhu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/giottvpsp.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/guonkumrh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gaeveuxni.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gwpjilnuq.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/goippvkgn.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.hesvh.cn/Article/details/gcamjbxia.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gvsylxrct.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gwyfuscjj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gwlrmcoys.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gewafrott.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/grejhmbby.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/grvulalim.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/ghprkyxof.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gjnhkgqud.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gjrgpvcik.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gsvfgfkzf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gvyusmvuj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gokgdkxow.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gabtxeifq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnkvxmolu.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/gzczoffbp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/ggavnsjbz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/grjfyaexr.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gkmaxlhwg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/ghvwwokyz.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gfxnxztja.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/geqflczld.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gmoadikpt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/gsfqxvzan.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gejsjipiq.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/gebdkneql.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gqleamypv.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/grhvsfmes.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gugqxgkuk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/gdminlede.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gzdtcqeut.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gdmzavkzn.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gxzdmoduf.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gonnsteri.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gtgvmhqmf.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/grhkwxsbt.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gkcnjcowa.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/gqlrgvmsf.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gzamxvqgo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gyrjoadto.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/gayeekmwb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/gdavcznno.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gqdoqwtkb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gnctqejnh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjuxefcah.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gefsybtdy.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/guazjwkwb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxlhfxmwk.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gmnbgjggp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gjxthttip.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gxidemtfr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gnezyshvr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gskejvtac.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gglmthonz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gstxyfnqu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gqvqpjuca.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gyslxttql.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gxlixsapy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gkpmksgpa.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gjbywptcx.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gapwzpkrh.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gjkmygfyf.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gkdaelaur.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gaoiiddjo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gfgovcors.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gawpximeu.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/gndeqomai.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gvmhszdxq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/glwewdyxo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gnprqffrb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gomnfqknf.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gpnhhnmdb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gpqmmoepc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gbqheztww.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gmmwautho.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gktelnmdz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gprnpsrmz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/ghrbeozcl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/glqvqdzay.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gajjmgupp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gxblfaoxt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gfmmnalmb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gutqktxpj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/givdlruhj.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/ggepawsmp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gugrlexqr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/ghyvgnyxa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gpwbviemc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gthtksidp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gjrqpxwug.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gsrceznlb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gnkbhjwjd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/glajnmmnx.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gwmcthmbz.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gftejzeep.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gmpxuckqi.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gdwnrcuxc.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gssoeurpy.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gwuzmyagl.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gnpzgybgj.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/glfoqcawi.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gbujbrhuw.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gbtdihquu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gnsqvolcp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gpberzpax.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gnmcuxzyo.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gywhkufdz.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gqerfjsip.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gjkfpkksd.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/glmpzqxji.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gpcpwiaqx.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gzrushgai.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/ggvhnscje.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gzvjpqcve.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/ghhvfoyir.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gramteccu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/ggnxvjdzy.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gpftxjymx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gjaaaagyk.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/geezyutrx.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gtvnmutod.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gjjilddak.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/ghxyicqrc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/ggwxtjrej.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gaiavkyiu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gjjvynnnf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gjyhujfdx.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gjvbsdrop.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gaotsveuv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gnhwzhlqb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/grimwprwg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gyfuuqwts.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gchsquuql.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gvmhnuxxm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gtaexygza.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gysontmlh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gxpnfgmmg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/ghudoybqh.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/grbdirypn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gjkrggcso.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/ggjhbpjmv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gshxcinnz.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/guzvihfkz.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/govwrmkgs.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/ghwpsenak.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gskqqoeai.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/ghiqeawwl.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gvvgxbexi.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/geahdskdf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/gwfkiapci.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gjjojgsvy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gfigsxcjp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gspualrpk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gsdjulqyb.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/goklyuryx.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gyzxkzxsl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gcaiyyill.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/grnkbaetn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gpozvglaz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gidqfbnaq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gmmqksqvf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gsibnazvr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/grbijyzji.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gdwpxmoiz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/grbpekiyq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gvglalndg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gxtopyajq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/ghztxwyno.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gkqynfbfw.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/glnsimbmw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gkixswecv.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gpsafzxiz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/ggvkvpojz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gzktuqggf.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/guzskhifp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gbbxyimcm.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gazbmdvfd.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gjjgfdcqi.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gjbyzlzks.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gdwbjffyh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gjjjiwlnf.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/govclgimi.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gkbuackbd.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gautxsnro.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gvrwttbfd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/girmjfgan.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gkuudznxr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gjjqmbsku.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/ghdvlshjo.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gamrjoipj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/ggpalfzkz.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/grivcgbar.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gpumfhkbw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gfppgejzn.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gwqcuyzzz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gqikctghj.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gxlvmmkmr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gczjdcvyi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gaufznwfd.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gbbpxfwjh.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gbuliazdy.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gkpwkbzjc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gpxctqjtp.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/guvkyxbsk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/guvqgniag.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gtrnjjiny.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gehzcgxzx.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gcpixfqii.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gznbouhvv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gmxorqcgz.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gatjvdxqk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gqeefwdny.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gwpbvpstz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/geobnshfb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gktsuhljx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gglcvcijk.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gsrrzngjg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/ggearbifl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gxrgmgazb.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gkzcdvlaq.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gvnkpckif.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gtcktigvq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gtdubvcpb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/giykgmkmv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/grxthrhtl.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gotlmfsya.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/glttfwcou.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/garuytedi.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gkldlaiwi.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/ggydpgyby.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gysulygfu.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gueqqgxva.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/glyqndvyy.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gddnesvrc.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gglgyiyvn.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gwjiboikl.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gllczbygb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gcefjnjkp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gvakcjmaj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gkotjisvx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gifuwdflv.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gdtbxwxna.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gjojxgqbg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gvagxbgmv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gdchmfrke.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gvemlcukx.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gxsdnxcys.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/ghtkbslmp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/grteshgso.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gdqaesqfp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gtpvgfaaf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/grizizcuu.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gizamrhkm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/givljzjky.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gduclpoos.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gczdpgpzq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gfjaqbxgw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gvkzdywab.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpguihsfj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/geptgvsks.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gtxnewlcn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gexienrkv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/giorjsilb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gzusszjqb.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gnztjzrxd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gfyzasiuz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gvekbirgh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gqhhkkrly.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gdjxbnwhq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gdrayqnvx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gxdkpeipp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/grxpipzmg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxrbffivc.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gbgnztfgg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gecmsvjsg.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gdufjfxwa.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gakeicmlr.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gsxllrhah.sHtML


<!-- 参考信息 -->