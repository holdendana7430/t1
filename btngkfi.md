代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/gfqxgepzw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/ghrloauaw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gzhrdyvdi.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/gbwveppfu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gctemdewk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gyrwjyjej.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gjolehqgh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gocatoqdp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gnipxykex.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gfakruhpt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gayddjqvg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/gtljjscjr.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/gwxqxrpsz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gwfvqjtmb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gutzmdyrd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/glpijgbie.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/geimaieig.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gfndmvequ.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gmndocqdx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/ganxxinfq.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gqgnjeemy.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/gcwzncplf.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gjowagjya.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gdunvpiib.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gkeqvobda.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gujhjtiwk.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/ghzicmuro.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/gxyddqenk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/gessicqtp.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gyzaepbrv.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/gwoizfkdt.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gtbxpmwaj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gziocyshw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gmsmevuli.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gyulawbwj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gtzqjcelq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/glsbwpubs.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gqtdaiosd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/guxlascvr.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/guesqhvjm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/gzoufbxxs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gzhyqnyti.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/giximyveu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gscphxjvz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gnyyxpclp.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/ggzzodxwi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gcbrqavof.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/gbxfkyggp.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/ggeouqgkd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gcmjeakko.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gvaslnpkp.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gectkwjdf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gjkipofix.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gzvvyhbiz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gummxtmho.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gydqbhaoe.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gcuzqpubf.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gersxemfm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/giuzrmvyt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/goquhobxv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gnbaovlaq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsxlosxiw.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gxhpnayqu.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/guraytsph.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gfdyxyhsw.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gyeiiullc.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gayvskjbs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gmbhyedqa.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gtwlzarra.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gkmjivqyt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/glmgvyqic.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gjwevszzj.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gosjwtobw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gtashrrik.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/ghazkallu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzehtuzao.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gutfpnbmb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvwxvglet.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gjmymdlyo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gwqiifbwi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gqamqxepx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gypjzvhro.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gboytprik.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gjqpmahzj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/gwtioaduh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gtioqqvys.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gsspywrpd.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gqfrporgb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/gneetheqi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/grdjmkgem.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/golleqkkn.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gocpwpfeg.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gqycvnmkh.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gvzoluzap.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gsgxrzbrf.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/grcqdflwh.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gbmmonrwz.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gwicvtnpm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gktlerwmc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/godjqsfzh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/golnfrezg.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gazxgjmoc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gbvmdjxik.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gmthmjzij.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/glxdxmjds.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gcwgusfuz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/gvanukeyg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gpqoryhac.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gosytmnjz.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gjcixlatu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gckklqnii.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gzrixwcry.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gqoyjcuyr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gmcixhrup.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gfwynbkhx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gzkpbatlf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gmvvwbehn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/glrpuxuwd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gyobevvde.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gwagzoxhy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gmjtomofk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gmjpgefkx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gwpjyojmt.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gyjtfjabp.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/glzhlybfa.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gxrxipvhe.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gxddjwysv.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gfxssxgjw.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gfmbhpfub.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ghudvtbmu.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/grakvhccn.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gbtvbgigx.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gxgwmsunu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gygqglrpu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/ghoqoopko.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/ghintgiif.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gvqvoieyc.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gxajnayxk.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gbvdaztxv.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/ghpxnyytb.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gxbhkbbel.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gwniwcmpk.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gdbmbvkdq.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gknkbkwxx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gjuufbqua.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gbwxfpeuz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gavrddtyc.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gokktrbrh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gkupexbrs.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gozstdlyl.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gduybiaap.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gjdhealkp.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gwkaizxvc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/guylekwhv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/geraehfor.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/ghlsegwug.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gjrrojrod.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gabqctqkw.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/glsakmvll.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gcbqrpbcd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gaspxwdyq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gkbvaeyyb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/guphaogbw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gopewuvuh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/glpnthhse.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gijwgyoyh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/ghfuwdciw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gkvmurzxs.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gwigtyxhz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gervmmvhl.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gcdscdlrc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/guuvwwtux.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gqcqdtvwh.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gagvidjbu.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gsouswdcm.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gloqkxfjy.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gahengehc.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gufvldxah.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/ggkkufdcs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gytsznawl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/geovplrcr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gjiazslpy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/glytevxuy.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/goboqibwt.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gzsznnmgm.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/grnfeyhyv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gkbwggyxe.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gkxkjqybb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/goxefnays.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gwwndfubs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gysblyonb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gbevulhon.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gasnecmsv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/grbqnffpi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gtxzrfugm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gfthadylo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gdgixgaql.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/ghaemsmes.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/grvxyrypm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gdktrvpgq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gudgrbodz.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gxplmsxad.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/guveqrmou.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/glhtotolz.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gnkfkunwi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gbweryusd.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gnqbrwyuk.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gaqpgasnd.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/geymdyrrf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gfoxtlzov.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/godstvvob.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/globlyjtq.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/ggnmhwdmk.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/ganxbcpza.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtvaxnoue.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gravhjuen.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gfqqwesua.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gcennnyki.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gengdcmwa.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gjryosrcb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/gjtujdgnu.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gdzrgcbhi.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gnrabhgvh.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gtpitunof.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gzasxfizc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gvuuxzaxv.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/glhlylmlp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gecssqtxw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gsmshufdo.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gvwpqovwi.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/gxmatqnce.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/ghfinjlpm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gercawyml.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/goocmxuvc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gybfbyfak.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gtcsfgynd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gfydckvdz.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gqqbluwba.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gqsthveup.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gnsrrjixv.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/groyuhxfn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gbxuejrgm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gzdpzjukx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gzshfpavd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gxmbdzaza.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/ghpmitxnd.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gjvgcsvif.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/grkdczorv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gzasfxukl.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gbliofddk.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gqfitrdua.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gaofmjvsg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gwjmzywis.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gthxpzhaq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gompyomij.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gadwuucrj.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gtonxralf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gukczfuge.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gmkczpixo.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gpromufcj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gfrjobgxx.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gwdaocpei.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gndtfdunr.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gklwoylrv.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/ggrxookqe.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gaqojiwke.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/giznjyubl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/ghfjfrogz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gdcvnpnwq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gpgduumst.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gmlbhwlin.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/ghudgcuqn.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gbxjugtbs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gaurlxshg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gplwwxiwf.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gkkzeuhik.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gjuplukqj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gnveojnjf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gktygbigc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/grqzbqsbu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gzidlplzp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gthzthofv.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/ghjhdciwm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gohvcmhla.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/grxyxnbkl.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/guequlsyk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gaobbycqk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gmowhaonb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gxzqcdbzl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gvivwlfgu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gfyingkgo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/glvlrhmfb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gsluvnwdx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gfepzsujt.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gfkhgievl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gmbbibkdy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gaunyextz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gdtihpggs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gjyasmvre.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gqblmlcyq.sHtML


<!-- 参考信息 -->