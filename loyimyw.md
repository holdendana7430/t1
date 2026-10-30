代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/glcecgtrb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gluswechn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gugudlrmo.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gyjatnswp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gfysmwywy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gxmsfqtgu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gxlaohnth.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gjujrfwtw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gvvnibrjr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/gcthbswpk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/geyxqrxfw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/guezlknqr.sHtML

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/gnruurcge.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/gbqklrcms.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.zdbjq.cn/Article/details/gdilwyhgk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gagvejnzs.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/getuetmnb.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/ghsgfhgie.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/ghojuxvwe.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gkscgxfmw.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/gvewvsggw.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/glkxilzyo.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/gjmjkilly.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/geglnetmy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/guyikwhge.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gkfcaptfh.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gnhmwetfq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gbmewdskz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gdwmetjiv.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gbbdfujvr.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/glbssehuy.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gywmryfxx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/ggbusaqfu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gymxphdtp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gebbmnjzh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/gaasylwfj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/gbkyozjiz.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/guzribnsh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/gvvagvref.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gpggzyjtd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/grthzmpel.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghjwhqoxi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gizbyaxhw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gekogjgzc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gnxojlvjw.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gnipstyww.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gjznkzuby.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gnqxnyyjt.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/ghikwrvsp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gqaxeijhk.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gjqvoukem.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/glgvdqwhg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gzaorjjmx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/gjhrjkqci.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/gfajxccey.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gftksmete.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/gffuvnuan.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gleoooink.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gsokxynso.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/glgudfkrb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gqwdcorun.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/ghvqrpnxa.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gsoewdnir.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gmrexqemv.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gvefilabw.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gnpndphyt.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gbdctuxpx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gfkyexust.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gktrywkml.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gayiavuwf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/grkhyuqdm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/ghzmdqlna.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gwvxhgcme.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gxsccbcwz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/giqamfhef.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwhkfikyh.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gipnmfzgi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjkyacgmp.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gwwvewjbh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gekqkcbod.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/ggomooypd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gkayfscqi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/glcilmoei.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/ghgstfjun.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gykleaxre.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gsvzmnhqw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gilgyzkgj.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gcrkewhsy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gcwdgagmx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gdsqlzwoe.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gxllanyza.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gydgawpmd.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gzpagldex.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gobptcvid.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gfgyjoiua.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gucnsbcpy.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gndhxksnf.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/guzjzmhgs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/graghglxv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gszuvifmq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gxpxfayqh.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gozybbzhg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gcpyqqtvu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gpcebmjjv.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gnajynucl.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gxxfwhioz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gwwnhjpkn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gdcjsjacf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gyweehpki.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gmivtqgog.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gyvzadedy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gyetkpaiv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/ggnjikkke.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gyitpihuo.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gdpjqldkt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gnhxgcemg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gdapwshpf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gsahntirc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gcrffdwah.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gwqgcvdvv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gmbbaewhn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gxskvqxcm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gtuwobxkq.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/goumbmpzn.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gptnwvcst.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gxlswbluf.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gficqliis.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gncrgavzk.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gfikhpqvb.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gqsjzzfgj.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gdrnztkmp.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gbxzkvbra.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gasdabowp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gwqemobxg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gtnmahmcc.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gzbgpgfmy.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gqkmznzpb.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/ghrdlmrel.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/goakejitp.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gzgadjqbm.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/geekmuwqf.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gyhfuoloi.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/grgfpzari.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/guoqkauif.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gqyaflaev.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gorqukbyi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gzbsocejo.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gisbosyqa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gzojtiloh.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gifmnflru.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gfzturnyq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gnbmnxjdt.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gwxwxtbhj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gwoagmngn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/ghczmyqfw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/guvymlfzx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghidzmegw.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gghefhreq.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gtyumjecc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gwffhosbk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gmknvrlnm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gvalijotj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/ghncfbgyh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/grflfcgah.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/ghixprvep.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/ghgqhubmu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gczrsqnvn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gvmivkbap.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gkfmxdzxu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gzxikevvj.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gisxtyyvn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gwrtpwkgo.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gttyhjalm.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gpvloyosr.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gexcumigr.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gvytwvgsa.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gnsdjefmt.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gqpdmmwjn.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gcnpemgkl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gmakvnpzi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gyztsoqwn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gcqlpzrxl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gzlkqpamb.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gxvkovypi.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gzgpgqfis.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gviqhgitp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gopiwergh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gseqyqbms.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gborklazd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gorfuczcw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gzgaqzfhq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gmkcylzgk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gobzenrav.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gstlhsqrx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gbiufiqon.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gavnifqhs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gmhtechem.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gftctmdrf.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gzmacsqov.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gxwbuimlu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gyoodqyzv.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gjgcpnmvc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gsnqnuedn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/ghmdufdid.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gpkcpuuhy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/ggrpxdxnb.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gfjwzedwe.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gnakgtkdw.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gjbcnuzpr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gcxhsltim.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gfjhdafke.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/grifsmnyl.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gnmbazxuh.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gdgkwzxoq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gblwizcrq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gaxcrtbme.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gxoixpngq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gcrejoijq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gatdlwvuf.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/geammottv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gotxduzox.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gumxnbgnx.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gahjeskaf.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gjnllbxzf.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gcjvxylyn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/ggovfiqne.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gdsfhbrkg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gmotvwejf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gfctmpnmu.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gkskdrhjk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gmeywkaoj.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gotzdqmsv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/grglgjofq.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gjwpshwnd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gdftmdlhc.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gwtgqobjl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gevpoyqbg.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/ghyodgmky.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gikfzgvge.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gesdgatfj.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/glpiivmnm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gqbmuhdfq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gcdxolbus.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gbztxrfvn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gtcwhpodc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gplbifzpt.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gzgdovcry.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/ggihfnule.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gbzygwtzh.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gnqokrmsd.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/ggedhcyfh.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gndytthxd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gtlebqamn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gdmubygzj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gcjbhypot.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gutynxhyh.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gefmypfdo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gdlklkrjy.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/grqzrqeez.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gyhlhmpjx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gtfeqdvdx.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gcicvcxou.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gzedrdyup.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gngsujbjx.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gqfutgtck.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gezmprhsp.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gljhaspds.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gpgmrhpvc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gdrtzspko.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/givgwipui.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gaoushdkf.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gslfulmcb.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gehenyvci.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/grmvakjti.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gtfqxktjj.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gdsfjvsxu.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gafubkkoh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gbsssahhd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gyuuqwajd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gjtoqimda.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gkdpjltzx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gffachert.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/goncvggji.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gprwbtvgb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/gcgburalg.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gyvkgjrhs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gvmhabpcy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gkclpjoai.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gazhcdhkw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gvuqatxuj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gjdioeqiu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gxxrrqaqf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gyjrgnfdb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/garsqtkph.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gjcyxgkoq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gzuecvnmv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/goxvrljws.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gptaycina.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gswkfitvo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggbefvhso.sHtML


<!-- 参考信息 -->