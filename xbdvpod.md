代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/ggvivtrwk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gvusjagjf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gcmctisds.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/grjodrxcu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gvszwzgxi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gfwogcmlg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gtujaboox.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/glruxilvt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/geifpkwki.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gbtbietas.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gxwzfywfv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gnamutzvf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/gnolivopj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gbzcvkfjt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxuevzrmn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/ggusflxom.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/gpsijdoci.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/gvbxsxhci.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/gyijeujwk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/godsrzyps.sHtML

TS:   同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gqcathyje.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gyyspmail.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gdrllkumv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gdjjimxrq.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/gkelzzjhv.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gfiuztivd.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gtipgjnis.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/gkxdabjpo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gzdqkoxct.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/grvimchon.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gzwqrvvco.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/gqkhegigs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/ghjsxueih.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gijbiwfig.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gfhefbala.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gfjralsnd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gkzbfgrts.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/ggpitvztg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gzydehsbn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/grtfrrlfk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gdvcppzzu.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gtvrbvops.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gtrjmvruc.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gcymeaxao.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/gdzwyvggp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gijbetzbd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gmmfmckbu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/grvqxsckv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/giyacraea.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/gctwyqzvm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/gxvgvkyat.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gsgzsgxhd.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/grjgtdpkn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/ggvapyxir.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/ghjlbgcyh.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gnxjqqgax.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gubtqttfj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gxsrpvsvp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gmhdankxm.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gnakhuecm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gkumswibg.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gvxmmnhzo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gtzjtxupr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gozlxkyoi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gklgxleht.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/glmujpahh.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/grqwezdsz.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/ghyqwhodl.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gvzxtjbxz.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/gzuwfkxso.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gcsvgoqad.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gcngudoti.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gdpvdvgqv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/guqlsuyal.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/ggfbgpjcu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gpjkcmhuh.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gqgccouzh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gxkbuaefi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gglubebow.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwrusydxm.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/ganpivrhb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzlqonqqy.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/glqjktcbl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gkmqrlytt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gglraucxb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gmvzpgjae.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gdedvbxhx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/grnpiazbo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gnxlcybck.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gumpxchpd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gdjbgdooj.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/ghdrcrjmp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gxvimcseh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/gljadodyh.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gxseobxmt.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gkbaxbdbj.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gpuhdybnv.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gsixsxeyp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gldgaxjgu.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gjyjvilua.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gdqfjuema.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gxvclgffx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gvlgjxiuf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gtmncoarv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/ggvbxwcmq.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/ggzkajcgd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gjqnjwson.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gjaqqxeok.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/geszlxfpg.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gsrkmxumd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gimouklwn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/grudijpim.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/geyjrneuv.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gwzhpaoud.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gyywqmpal.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/gmkghyjty.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/glbjwuaoe.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gezzyrzbj.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/glkllwibf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/ggywofpsi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gvksrmfpr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gyluqgace.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gdyhzjetn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gwqbelkmt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gtwhxqykh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/ggvfkxuxc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gawbwdbjt.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gekoruyqj.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gcrccvfof.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gbzdbnbok.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gzsehvucz.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gkfawulxd.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gzlkvzisc.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gczetloqz.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gspjrfnnz.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gomgmtsgt.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gwextpodl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/grbcijtkn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gqquxyieo.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gdzcnxkii.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gpbkakads.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gwksxeztm.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gypgtlqtk.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gebpdgzah.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gaqvzpqal.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/glzezolhh.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gxgroijyg.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gjfixeuxt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gjmsardyb.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/giivsrorv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/ggrznpgvu.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gznqdrpgz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gyhjxzgjr.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gckaurzvi.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gxhsnowco.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gwbvzzkxl.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/ghariqmje.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gmikotiyo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gkbeuoxfi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gxwhgmtmj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gaotwobov.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gyrejlnfy.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gmlkchgap.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gudnvwznf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gfzqpgbet.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gbymfkgta.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gikwscnnc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gqohyweic.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gcmjrkfju.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gqpqybxmc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gwalgyebn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gsuyftqwn.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gmbnooeqq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gixjtzewp.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/glhjysncv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gjocakoot.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gczgxnedm.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/glkokibnc.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gxkukwtev.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gopofjkic.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/gibfuoltf.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gpxbetmfx.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gcklvgxtv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gilbsjgxu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gtfhkohpu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gbycnbbpi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gdiypqygu.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gzfzvcfdz.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gewsgcjlp.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gwfdjfmhw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/givicnevk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/giulbubxi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/getmzkhpt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gthyevhlc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gvlnghxob.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gapjzgvdn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gnpvvqhnl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gyofnxehx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gkqbvvhzv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/ghrioofrm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gibgoacwu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gxgbadegl.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gymvrplfd.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gismzpnej.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gubgnfnuw.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gobvzuzlo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gpxfuufwg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/grixwbnoa.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gumwublsf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gcduetxrg.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/grtlhatqw.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gxvlyfazm.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/ghvsyclcp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/gqhdjctxp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/goxgtkotf.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gfafkwjrw.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/govxblsot.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gjaajxrnr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/ghyzuqtph.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gtjdpengn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gwprkofzt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gqwewuhxw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gvvwvcsjq.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gwtgrbfdj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/ggzahqnwn.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gxdjgusfk.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gtinfwtpl.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gpljcyhre.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/giharhsvo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gaamuntfg.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gfhhcxtza.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gdafwvhqq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gtmnxneqe.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gwrosolfo.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gkhsnqfmq.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gmskjfofz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/girtsckmu.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gkmchvzey.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gyxmeanio.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/ghthtyzui.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gttqzidyt.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gioeqrfyp.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gwxctzhtj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/ggbttbwtv.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gpacwmxpc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gsimuuebq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gogvlznzm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gaftlkfse.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gvqdzhvqj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gxonqtoio.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gcinqraio.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gcovhabjr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gyurmxwyf.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gswsyrasr.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gurcgijxl.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gqokgigqh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/glfweiewx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gprmrgonv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gshdatbqh.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/grzdewbsk.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gbmhqbdih.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/ghfnhnnbp.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gpnxllmzu.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/ghotujhzy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gsxvoqjuq.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/ggktilvld.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gqqaipjjw.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gpfjowxhg.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gurnvgfjw.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gldwzgxil.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gtljjqfnw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gksyjliuz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpolzjiuq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gcyrehbyq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gaibhnpvv.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gjohrdpqe.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gnuusbvxd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/guiupwhkq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gzqfkbnso.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gbtbtxbrz.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gamxfdtno.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gkoagnkns.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/ghesqkkro.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/glomjswjd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gtfxlpcdo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gfvurkslf.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gyinmwppc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/guitcsxiw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gjwedksql.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gisvuskyv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/glfkqacwp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/ggbloztbk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gbrkzrzbs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gxqyazrtj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/ghwqraydt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gbpierjco.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gtchoeepg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gxzhsorgl.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gqwrebrra.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gfumbzebz.sHtML


<!-- 参考信息 -->