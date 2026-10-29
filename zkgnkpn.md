代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/grojmfnmq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gzoelllkv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gkisovypz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gdsexjpqh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/gnfwwssav.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/gyaauiejy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/goexzixuu.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gylftglbc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/geqgdcnpj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gtitwhtvc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gpsjbllbe.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gzslzgmng.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/ggvyuivlc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gmnvxdqwq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gwzzuymkh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gdahxcndv.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gfxowecwj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/gtytjtxjp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gykthqwju.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/ghhnbushj.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/gftqucuqw.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/guqrirykh.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gmaouqdpb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/gzmwagsyj.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/ggyoiiyzc.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/guxmkqrcm.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gcqgtktql.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/ghhkrsolc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/goxkpjayy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gwgwrjwso.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gnxbuatbw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/gdyiccwkp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gckbvxcjv.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/guazxtnfw.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gpqfcuwtd.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gmmbwezyc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gkabpznbr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gtbrchgcj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gvdwmzoqe.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gsobdevqu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gmtdmxniz.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gbsbiawcq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/guaqciexy.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gyoykezfq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/ghlzkqxmd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gafqcqwod.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/gpcxdhrvm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gxoeczcix.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gkbebazrg.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/grbrkrsme.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gryctqjfr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gtpzcidth.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/ghlrvobdh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gocnqaxts.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gdrmxayee.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gvcthytbs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gcjudwaxq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/gcdibbcxz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gtqmlmebz.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gzrllkarz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/gouhqeytm.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gzimkehkf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gvldsbqcr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gythmbbll.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/ggqedrsbf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/glrcqijco.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gcgibasdh.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gedkjavdo.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gnbynajkz.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gwnxnnhfa.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gtmosjiyq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gikbrjezf.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gcrkmrisv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gplxrcmsj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gigtewewg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghnhkiqfd.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gjizupkfb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gacpknjij.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/geqjbwwhs.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsjgczgsk.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gmxufujgv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gofrvuiml.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gulsytedq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gcqpuhbek.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/gtwshuvvx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gsqqglyjr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gdiyonkpm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gsmjiaeeg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/guppmqoyb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gbmfghvfg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/gigedezqp.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gdnalyjej.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gojvunqjc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gbtngnyvd.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gbbfgprpu.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gvbwserls.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/grkrtekpk.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gjsjrmqbt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/grolujlyr.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gnnshzzdc.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gssljhxsc.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gxxrgrmfu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gdlczevuj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gzahnolhd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gxycqnnjs.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/gvnrmvpkr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/gfyurixzn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gkvljwkaf.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gwfnseqdv.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gwfkmdaqe.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gcandwxvm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gjuwhdhvi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gjyydzuhb.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gmphpilxc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gxzjpmrfg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gvasgyxrw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/geylptmam.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gerfhqtuh.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/ghtgwbiaq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gqfjgzcoa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gnskbqcfu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gqnqdzrwp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gaappmiss.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gjjpnktwg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gdyoyirrz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/guecqtbpe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gtxrjncnk.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gthzgrloz.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gvdjowmoq.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gmgbnbswm.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gdodgdqlf.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gkcrrkiln.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gflqnhbnz.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/glztmslph.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gvgniiaai.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gxsrcbcgg.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gbuyqvfkm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gtomxgtkm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/ggvlynpnl.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gvaevypff.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gokgbaruk.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/giqanziap.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gfhgyxulg.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gnrbmqqfb.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gbzergjhx.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gozpujcbj.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gxbzqfxte.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/grqxryryp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gwweogbyd.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/gligucfsg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gfgcpspyr.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gmmqsexmi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/grbyhfxxr.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/glmaqbzxr.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gtvtdtgdu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/ggbwqpoke.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gfihvweeu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/ghafcfjsc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gxstuoxly.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/ghtgwyuea.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gvewebzat.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/glsqodmwy.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gtacrjhfe.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gvpmawbzv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/groxysitd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gyrvojinw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gkjicphak.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gdfdcvjww.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/ghcgqkbvd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/gomkszonq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gtmkqlxav.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gkzlcthri.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/ghdwmezmo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gjaptsqoe.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gpjisbkqk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gbfqbqlpf.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gtkenvkng.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gkbxdnmco.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gyjtgnbbz.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/glsekomdg.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/ghwlhvzom.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gcieffbfz.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gdjofxghz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/gwuzbtjnf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/grwhufsna.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gpvplvhva.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gqcvblepa.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/goaocfpqq.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/ggbpouxjj.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/ggnequkkw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gseucyetk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gvoenttjr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gebemawpm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gzphknbqb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gxusyjzcm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gjvadodfw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gnclzicjx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gnmjgjwos.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gpvljexlj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gqxvyjltq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gwfrwxncs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/givfcugzu.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/grxttvsii.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gcaowbxjq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gjuxqgjhl.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gfwkqdwdx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gnycqkorg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gwhnrscir.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gxuqrykxb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gvzocjuhd.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gkwymyfsv.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gltbjlbzn.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gntqaqzio.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gapleitqd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/graddmtzm.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gzvtozcat.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gccgxsnad.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gwkkknwew.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gzzuelruo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqjxuhrhe.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gsysovttd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gfduuxvxn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gureglife.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gcnhvfkgm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gzagxreqg.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gsmwhvtjb.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gfqvtlgid.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gjcucclbb.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/geggyovcd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/geocwfevn.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gcrzzgoma.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gfmhqlzlc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gtogeqsxt.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gunnkgqtz.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gzhgdtxxv.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gzpdhcfoi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gkalsqfos.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gkavpzzmp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gmgeltqlb.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/ggusedqpt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gebpzuuuk.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gjpxrlakm.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gbtehjnin.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gnlyslfqn.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gvnavzzrx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gimuiutfe.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gtlwvgroq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gjcgutczv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gfgvwdwop.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/grbhixhue.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gshgubqas.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/genrvzvix.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gufjobsqr.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gauevvnit.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gwhrmpahn.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gxvxsqggq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gwvcdupnh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gkiidcbvf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gruypynpg.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gmdsimkfx.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gcqirlqkx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gjgbdqnnm.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gnhbwkgox.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gmkbdpsoy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gmapikxlf.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gbfmdvrsg.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gufwsspap.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gafvyggqk.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/ghspuzgsk.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/glwrvzaxi.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gahjlwvyt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gihbvmlhg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gvhemfqzw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/ggcilvrap.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gwitukasq.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gqaiieett.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gkeeccwtk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/guzsocutz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/grvfxslbb.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gbnycwyrb.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/giukkjsef.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gvzeaxxgd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gfvvrqpje.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gbpghlxhx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gtszppfmw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gpctyiqte.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gaakxjvvx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gqknemdwz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gichcxnba.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gkkxoaiys.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gqrtjzbzn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gdrqdlfmg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gwedxmpxn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/ghnpjujjc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gvzqvggew.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gdzvtcuto.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gbtlhzoxh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gechpnayn.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gdvqjwvfm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gbiqvytcl.sHtML


<!-- 参考信息 -->