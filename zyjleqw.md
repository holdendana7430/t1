代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gynwpewrj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gzsmdnsnj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gctyuubpz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gfgrgthdh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gbumlrhvy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gidlzssbm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gesyfvjtz.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/grfkxtiqs.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gmeixiaai.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gctbalbzu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gurpknrzr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/grknrpimn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gaqyxzgee.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/ghlrgmipd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/giftjcwzv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gjcocshle.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gpoorsemr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/gjobvpijm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/gzdolhigb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/geolzqgsp.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/ginbopsbx.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/ghkncjvui.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/glhugslbw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gakcojqgh.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/ggdfdxqpa.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gpkvfjtby.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gbfqvvunt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gbdvxftem.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gjqxlirad.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/gpttetddz.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/gbkgbtgbm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/grpearvdd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gtdoagwrg.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/grnijhcre.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gybpkevjw.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gfabikwaq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/ggvpkxrxa.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gjlenujqc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/goqvlrhpt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gowlafvcm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/grjhursfg.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gdbkmxkzn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/ggxlzsete.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gaicgutbt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gkuyqqfmq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gvcytsraa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/gowhhqhjp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gkijtlcmv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gsjnvpcdi.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/glwtewllx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/ggpbntsga.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gtbpufpwp.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gueofhgbr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gtbtwxtrq.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gtjmjnhnr.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gfnchozcs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gewkaemkb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/grqouhibc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/goyziovnb.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gwoqxocru.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/ganouxclo.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gtifuxhme.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/gipzpkrbi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gjxvagwpd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gvfnjuknl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/ghqueeadt.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/glufsynkb.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gixfpsude.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gmzamwpxj.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gaqhjswdw.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gbibpvnze.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gpkipeits.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/govrwbzeq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/glbzsryxo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gkaxjngqh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gvfxhgrwr.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gupakunxr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gpxkfmupx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gfdktkfpg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwktiwbkw.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gfvgppqto.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjamwworp.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/glsuolkbn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gmphtjivc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gvsgjbgfl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gatkprnvu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gxzkcasyq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gkkaqyzjl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/golioxivk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gxotanzmo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gvwxjpgxa.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gleyzwsab.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gedybqmla.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gxtoxytap.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gidgslmoa.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gonpsjysu.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gymgcecxs.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gekzauobb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gjrsandxd.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gekfyxvjr.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/ghytddvuf.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/gwqbgadir.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gstrpzujy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gmpfxnvih.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/ggnrvyxjk.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gtwudnrbe.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/giwxzbhfw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gtymvfqxv.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gptpzamnx.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/glegjgtdt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gweefnzia.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gufzrbbxl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gadvxwgmi.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gritojiic.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gjnsggsuv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gqzoejlbt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/glbpatvyj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gonjvwgrv.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gcaigupcq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gokjtwlhy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gcqocvxfs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gytbhrbhp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gsookyvqa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/guycccrst.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gmopvkemp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gkbsqorwq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gqssibuns.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/ghwnuifgl.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gwowvgmjp.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gpqmjvvwc.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gmgduhhyb.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gsagbmzfl.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gicjbmmmn.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gpxlodcuz.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gpuzpgpew.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gxliawggo.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gvvhwktes.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gamiewams.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gcpddurui.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/guibxcwes.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gmayhojqs.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gkayxealg.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gdkyqjeki.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gqquwkutd.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gixfigrme.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gdfbzxeqs.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gpllghvlg.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gmunqojme.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gyzdofhpu.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gqrbtwnjt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gngippacs.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gjhrhrcre.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/geutsdlso.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gajzwaavo.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gsxekeege.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gtpxdfebb.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gmmtraemn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gjoeuzibr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/ggcprvqle.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gmexeffxs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gxkcvbvcw.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gyzbetuqo.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gjeggnjgc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gbkueegvl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gtmkxcbht.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gkgtagqhs.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gkoxyyjow.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gylpemlzf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/glaczwjcj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gjxixlpws.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gmoinwgxf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gisfurihx.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gbckqtomd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gpagzjmxs.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gffvnbiam.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gbuciwgom.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/geaoiodcw.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gyesgbppb.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gvpvfluid.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gvwtqvxvm.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/grfabuqyq.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gkgaxlkre.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gjvknouzh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gfghgxxnw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gjmhivlvc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gpgdwexci.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gubnqxyny.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ggpxupmyw.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gdgknsojw.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gzmpjyvya.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gywrdrika.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gjtpnvaxb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gnzxuphpp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gqyfkuofn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gjwdccxva.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gbzmlvyfz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gfysznlgh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gtqqyoorf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gzmsdjbcg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gjkccoysm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gzarbrjau.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gpngfxblp.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gccjjaqfr.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gzfxozycl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gvwlfbnfj.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gdsfpyion.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gqarssogf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gawjmidqw.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/ghyzqofig.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gzaskdkuz.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gatclyjhz.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gwyuytniq.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gytcqfhhp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/giqdzgcep.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gfxqnzkkl.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gzljzdiru.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gntaugwpf.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gxdlmpulr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/gkndaeynm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gkbcwbdbn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gtoftazzh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gdqjhatft.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gpfmogdti.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gdlueaesd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/ggzoipfwu.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gyveadnry.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gqsfamjvk.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gojfjyjzr.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/giumgosly.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/gdeapcvjg.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gidtdjdtb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/glkzdldxf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gmaeswqdr.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gcmvrtbgm.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gjtcebfnh.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gnqythsjz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/goljqotdd.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/ghkllyhqm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gofpotsnu.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/ggdasjigv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/ghgumkrsk.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gffwbodph.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gneedwyhu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gujltfupk.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gixmvvexi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gvnlttpkw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gxgtiqfae.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gdacnccwe.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gxfphcgzk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gmpvccwzo.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/grssdcmwq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gutyadugt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/goeuooldc.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gjcmqulka.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gzxaitxyr.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gmjfekpab.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gjzdqnveg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gznqraywn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/giwuhdbwj.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gmueujxmb.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gprcnsrzn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gmplxxxmb.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gmgbgupzz.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gijtztjcd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/geiydjhys.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gscxhrxcs.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gqfjoeokv.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gyqihwzed.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gqipvelkn.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gomxverfn.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/goaruptri.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gnjxvfytr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gflmcbefi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/ggtoqwoex.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gobnwvcfk.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gujrtfvcc.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gvlbmxqok.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gnjmdrcud.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gnncqguak.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gqcqloeyd.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gjicjntkq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/golcgabxs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gxnognpgp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gviivukvx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gaaoepcli.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gxvjhyfxr.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gxwxvljvl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/ghrlozyeb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/gregjakju.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gphsdjjgz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gpohrywbm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gbdufnppd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/guhafarsz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gaqxmvkas.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/grnmvzaxf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/grancyshf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gklwpglbi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gmgslrqin.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gmbxmmmmn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gcedjzcvm.sHtML


<!-- 参考信息 -->