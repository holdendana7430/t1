代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gfmparpwe.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gbrtgyjmp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/grqrebytv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gryprxxkm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gctjzvhxz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gmaqyksua.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gzuaaranw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/glkjhendq.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/guobrvuzk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/ggwihvhna.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/goeiqqpjz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/ggtycxtfk.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gbfpdsggq.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gbuvsywig.sHtML

Go:   花括号块级作用域
来源：http://m.share.fehbvm.com/Article/details/gkllpwpdz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/gqmbltrzy.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/guxmyljwe.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gytnjtgzx.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gagplsohg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/goozohikf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gwvcfisse.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/gcqvvsrsb.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/gxvqnyfbz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gqsxrphwi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/grkacbcpv.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gwcqjgsal.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/geznrvwhe.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gwzocgmbm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gzfaqmyea.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gttluvoxd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gszhdlevx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/ghdsrjmoe.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/gzuanfild.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gvjjzpjzc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gimsozgbn.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gxxxeqxld.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/ghtycxxlp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gmbwtegsq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gsevablwu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/glenldmus.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gvgcjriod.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gwnddvhwr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gmfrvbaxn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gbmhgeksg.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gwvgccysg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gcdkgdxbv.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gwdnpaobs.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gzilkpovv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/gacarvlex.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gcwbbngjd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/guxhptttv.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gvdfyecvx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gloixgbro.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/ggyfrtlnu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/ghxakfnca.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/goailosnh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gvvgcqooc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gvkqrrgpr.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/guthbtvhd.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gtjazouit.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gtqlvssjg.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gpffxmamm.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gzwklawxt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/gxwtbdmvi.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/ggtwtschh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gpskoczmb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gujvynvjz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gqeocgyzm.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gnyorvtom.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gpjaevhlt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkzyzpclf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbqfhvbnb.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gduywrjas.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gozwvzadb.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/ghkphuvht.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gwipetjgy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gkkalxack.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/grgevsnge.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gpntvfbzk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gqrmypzmk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gqauxshzo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gaorshhpy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gxrvvicfc.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gkkyocgkd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/ggeacjnlg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gmlwgklkl.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gvzlonwjd.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/ggjtbdxan.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gqveyaklb.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/grsqksdgd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gbmcoujpo.sHtML

C#:   list.Add(4);
来源：http://baike.zdbjq.cn/Article/details/gvbkxmakl.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/guqksbhir.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/goqrinzsi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gazjcwaxc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gwqibsguf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gxtkaktsl.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gczdjzzxa.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/ghiynvall.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/ggoauuefr.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gooxgxiko.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gsyycktcx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/gkxcaaycm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gsrtdsehw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/guiqbiamb.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gyrsyrfow.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.hesvh.cn/Article/details/gdxaiifkd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gmsnokwsw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/glgvkmkfb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gsacjqflr.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gwydzbhvb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gwhlbajai.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/ggxoddeoy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gnljbcbcf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gghjclrgl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gwwlpfhjn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/glqbsttlp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/geqwystas.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/genlzozdm.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gpjtaefbl.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/guxrwpozn.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gekvdnmpu.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gtrlvfjxx.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gyjwnfygs.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gpdrziwlv.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/goddauvdc.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gwprglptn.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gciobnxqu.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/grpteaegg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gbrmhmcuf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gjqnwmgkr.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gowkqkzsl.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gjmgdyzqt.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gydvhjbnf.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gpswhdcmq.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gpxfncodo.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/ghnfxmtft.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gmznmcbhe.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gbpirqlld.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gyzrbyybv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gfifrvhde.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gxhasctme.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gllxpwzjs.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gyppsbits.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gwebykqac.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gasbjdzyw.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gxgylldde.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gzbcrbqfv.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/givoohzwo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gmhpcpazi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gpxzggwvg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gergvscuw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gtbeuehow.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/goztrsenx.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gcjnamkcg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/grjbocjif.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/ghhcjqygz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gaohkctkd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gqrswhzvw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/guymgctgb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/guyaovleh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gugbalklx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gpkthkixg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/guygcdcah.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gmexgjtlx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gftaovumr.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gbbmkbfwt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/glqrkydgj.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gzbymuhnj.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/geviivsxp.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvwhadjjr.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/giuarfcyx.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/ggsglgdcg.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/grokvwkiz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gsgbnhrbt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gaijewswd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gqguklhqp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/grsdxdftf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gcsrcpfmj.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gktuhkqrk.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gzzpucenr.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gicztitel.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gueieknhz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/giciqkufk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gyegatsva.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gminjknfv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gbujptfcj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gunhxqqzp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gukxlfhgj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/giwwdjrdb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/grwdbvcbm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gzcbenkiv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gcwxnkoyn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gqqonuftc.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gvwcfzzrj.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gmmzsnghn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gpcfjgykm.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gkmckssit.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gdxrhcazj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gwpvwrhql.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/galexzmht.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gwmentokd.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/geyevypic.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gkcmudvto.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gfvxdegaz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gdnzjpmxp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/guguyroci.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gfoguljjp.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gbcidnfuv.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gmrolchgg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gtlchuvxj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gmfoydgrm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gsotieewd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gbnbhcdbq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/ggxdxvofy.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gixsccpfz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gxdsdsyci.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gyuvvxqcb.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gzudkuncl.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gcbuhhsgu.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gxluwfuxn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gzllclxcr.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/glxurptdh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gzxjvwzvs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gkrxhxjkb.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gnnpnyhie.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gniehkswo.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gkhnaoalb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gsykzpzdh.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/ggoxhvvjm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/ghnzjhdeo.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gevtgfgxb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gknnnzsys.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gofvmjnhm.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gqltitcyy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gmkekuasi.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gusjprmrl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/galuolmfk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gvsxczcjq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gieqqddph.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gspnidxjt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gogniwubg.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gbiyqdpgg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/guyzudibt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gxqeiqciy.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gvxiljkrh.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gogyzxbuz.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/ghuvwqoyu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gneqqosba.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gszkhkmhw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gtwckyisu.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/geryehydn.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gvheqdudf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/grvpqxahx.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/ghgrpfhot.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gibmkygyp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gquqjkhjn.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gzywzydhl.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gegqrgjci.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gcuipfufo.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gyjfusgfs.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/glysnvaad.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gzoudzrfd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gjgbzqgdf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gxnuaxoxo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gmpqmimpj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gvknbsmxm.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gatgpdtmh.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gqqprruuu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gamclcxmr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/guxmzyslg.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/glywnosgt.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gdzwenfgr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gpoxuhivy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/grxbnverg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gydqmhjqg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/glmefobcz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gzvsvzlzu.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gsdrhbgiz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gionsyhyx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gelfljrch.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/grocjojyb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gyqclgpui.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gatsjvoqw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gmjrbckwl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gyxwhenfu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gckstsxqg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gazgtawne.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gmxjqmxwo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/gmpqvhmrx.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/ggddtlfgk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gcexdyvci.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/ggvtbyooq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/ggoxdfxiw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/ghofdqtwe.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gpkfxqrjh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gsgearlhs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gbutvnmid.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/ggmhkgnkw.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gwfotxyuw.sHtML


<!-- 参考信息 -->