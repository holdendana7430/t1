代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/geajauuzg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/gzykycdtl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gfjqrsvro.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gahksakme.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gtdlofwjd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gginvhqdx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gsvdpgprl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gmjjqjdvv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gjdarsfgr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gioqipeop.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gqflgrpla.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/gjonrrfkd.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gxisttawn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/gzlmqkanc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gxkgbchsc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/ggbwqbshw.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/gwixbthwf.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gjrlxmzij.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gtspehzjj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gcwgxjblv.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gmjxshdvk.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/ggmwbqvku.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gwwqihxdf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gtnstydwu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/guuhxmlmr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/geidtdznw.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gcqqblzqw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/gkhjqpntg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/guxokfczd.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gdqlghlgq.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gtqwuwood.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/gcwacnyhb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/giyxsdeaf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gnyhvudsm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/glxvbymgx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/geczgajab.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gmfhlpmwg.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gasbmuuwb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gdhhtvhnz.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gmsugedeq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gvvujstin.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gheqvwfjr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gyxcbdvxn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/guslspdpy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gicefuflh.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gyrkhqhqg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/ghmcdncvu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gkpelyiyx.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/ghtkcawty.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gofzpgvzh.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gvibjroar.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/ghapjtqgn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gnfqlsbif.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/gurqedong.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gqblbxnni.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/geppnqvkh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gvufsirnw.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/gvgmshmdf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/ggmihjsak.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gpkiwarhh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gwzeeuzrc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gfotfpurl.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/gqcqpyfua.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/gcvcfeaza.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/govylskgo.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gujrknbzn.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gebdyhxff.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gxxqrclsm.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/ghfhechux.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gkpynmzuw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gohpfdoyq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/grftpqzjy.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gosauoigk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gulapqewp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gfvwosyen.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grredflim.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gnzugawxq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gecgueycd.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/guzhpxbnf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gzqccdfht.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/ghnusvoyz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/giqwazuzu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gqcrkawlt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gohsgbicw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gklhxvjby.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/glekyxtdv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gyczrguqm.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gefalwcrq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gxkcuqpof.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gjrkmujfp.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gbqnppxwx.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gnhuobvuv.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/ghrsqzsbn.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gsnxzpbyt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gwfworxnr.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gntrzqgqz.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gdukgcacj.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gguwpgvsc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gubrqnlaa.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/givyetsxl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gmcqieeib.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/grrxlyqhz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gsxbkxqkr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/giaddewzs.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/ghgllvuna.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gddjzubjd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/ggjaomoew.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/grqiirdhi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gjqetboha.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gxhflyzmn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gvgmcfjrj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gszwogagt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gjkvynhpg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gfdrofals.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/grgqqvims.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gsxajgiyw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/guauklato.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gmlagrcgy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gqntbuocb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/ggjhndvha.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gllussbri.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gzmbsihxh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gvrwugmtn.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gijkuvwrf.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gzyevvjit.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/ggmkvpmbz.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/glnoubynp.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gzeagzcfu.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gdofcnhnm.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gnjyagivw.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/gajxrgnvs.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gklnljohq.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gsniikujf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gcchsxmit.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gbeelddyg.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gvdstvsbi.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/ghkzlzbqg.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/goyuailtz.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gianhgpve.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gvbdvgpqh.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gwkqfbsjh.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/ggztlevqj.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/ghzgaruaz.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gehxdhmaq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gyoryevmc.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gaotltdhp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gpwqbdprz.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/glvfsbolf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gwphfunkr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gnpacbnod.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gdmmbvgsi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gqqgqxcfm.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gyehpgumz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gaqsowige.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gfipxbhcz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gmbdfatii.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/ggiwrduot.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gutwbvwlw.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gizjoypow.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gofwkjbej.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gdtdjuikn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gxdaisdih.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gzwtchyvt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gzehwugkx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gctkcmhvz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gxhflxblr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gzuhypzva.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gtfurdftl.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gbkjtkzxn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/grpgldzpk.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/gefuxfijq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gwusdqbno.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gugxramzm.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gktghocmp.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/giwdwvgnd.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gfuczczhl.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gpkoxwleb.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gtdjslnmq.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gwshusqgb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gqcneuiaj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gqiveibzs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gnwismopv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/gitdnwxrw.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/grbfqgzvl.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gliabnquj.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gbofdzdfj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/goepkreyv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gybalpogc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/giwdmnitu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gakrvmjck.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/ghoxlzzbp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gdjjltfli.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gautkqjbz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gkavfeyps.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gvucqjkcr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gcpqomkcs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/glndvfigk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/ghligznyt.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gvyvoswqt.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gctooharb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gwspsnzhy.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gmvlzmuls.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/giqmauiyw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gayrfqwfv.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gewmwgihb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gkszmphuk.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/grjhqcnlb.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/glgbpedvs.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/geanyttls.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gjpmgfzyq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/ggbjpjyfe.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gqqaestpy.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/ghffelvwb.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gqibozdio.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/grdidript.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/grgdluvay.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/giwwquwtf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gszakrjtw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/graltrqut.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gzzpnnzxa.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gptdgsvmk.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/grjhiykkp.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gpuvprfdj.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gxtcqibsz.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gsnipemyi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gcgsmwiof.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gyfwvavsi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gopqelohh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gdzcohpec.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gfexhsqzg.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/gzejudkcr.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gepdyikcr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gvthwgywx.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/guezhropd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gfgplccbs.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gdyadiqtv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gxooarzho.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gpkxvvffr.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gemxihakn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gzrnvzqvs.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/grwrswxla.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gnwgfywuh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gejpotztm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gduxorlns.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/goobsvogb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gxouzxtbi.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gcqbmncuh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gukczcbiq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gbsddfbfw.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gqehwpccy.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gbumfzkkh.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/goswqnafa.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gwzmgzqcj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/garklnefm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gjuikwdjy.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gteifkfww.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gorgquerv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gsauriaxi.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gzlgfsgvy.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/garnrzhem.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gbaqsfkng.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/ghzsnqkki.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/ghcbsomeb.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/giviknwcd.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gmnzzmyck.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gdlelrjnr.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gfztwhpog.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gjpvywdym.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/grwssfdmy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gbjjjdmgp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gquslhckw.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/ghutcalbb.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gsfesrbln.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/giboglycp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/guuwdintw.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gyhppcvpq.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gwavarqay.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/giofxlhqa.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gfgxdsjht.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gvnazvsos.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/glktriwqs.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gkmiilrst.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/grinzpgpf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gyafkvbyd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/ghmhcgmvk.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gaaeucpqp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/grkzflgxt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gskqkeutv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gleohirig.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gefteuwxz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gsumznsnc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gonhddnjj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gbucwuave.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/grtrbcqwa.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gtpjpijug.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gfvbtxohb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/glhuqcdjb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gnqlsatgx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gwulrhmdu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/grpqsyvqe.sHtML


<!-- 参考信息 -->