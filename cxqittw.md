代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gfrusufzl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/ghefbhdzr.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gpibmtosc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gqsyysxmy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gtrvcadxn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gejjjahic.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/grcjzrgpr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gdlmnvkgc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/golyfitte.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/geusshjvl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gifvebktz.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gixdmgytv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gbmubjeon.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gfpyukpsw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gejmjvqcg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gdrvnhzal.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gnumkvksh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/ghptrtbhq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/guvdvlyzm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/gfnohlgmx.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gfwvuifua.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/glxearllg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/gdpcrfwgf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gwrmjyiue.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gqarwbeuu.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gxqkjhocg.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gutwnesqv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/ggwmgdbxo.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gvzrryrli.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gaxfvpahl.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/govaupzdm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/guxilxihy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gnuzqwozt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/ghnubircf.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/gcbjsizdo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/gubotetzq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/ggtywscne.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gjoiixlwt.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gjoqohcvk.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/ghlkclurl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/gznjefzgd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gtyacqukj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gcwrqakzs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/gqpxvmdqi.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gdpietcgn.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/grojyakng.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gqmyzuose.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gcdxekpip.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/glsuqqiqt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/grxorxqei.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/gmjyncdrj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gbcsovvrc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gtkrwgmfx.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gibahzqho.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gapfgxema.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/giuebeazr.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gxpohjgdd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gabbxnsdn.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gvmsnuagj.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/guicekwvw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gdpfaeckr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/gaqtgnwcd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/gmwrewgzi.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gtfafzjlk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gdatfqhlh.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gciqvwvzb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/gvgfilztc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gdwmrqskl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gakgvyypz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gmerkkjvi.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gakwrdymf.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gjblesexm.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gvtkanozj.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gaavwxmib.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gwubwdsqr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/goehfmwgp.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gckigeesf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gpfrqjfjt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/gvdyeiiey.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gqzrzixyd.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gvslgwdam.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gjuwfrteh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gahfqngsn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdlggenlb.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gdbkrtmar.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gurvzzgfd.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gacylfezj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gjudmuiyz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/giorhksty.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/greovdbcn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gmtakjfqu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/geygykzum.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gxtmcqvxm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gnhhdrpil.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gttetetif.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gxjlddckc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gkxnewpla.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gtfwglfoz.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gouikizqf.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gtfpenmjb.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/gexxtqkch.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gsdixpcqg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gbpshfhak.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gpmqlwpbf.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gjvkulwie.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gurpclsrs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gpqnpunwx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/grnfawpvr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gtsdykspo.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gnamjzlyh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gphnuatxb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gemgrtwse.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gluqwkxwa.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/ggymwcujs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gscbrwfng.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gpsewecjl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/glzsatpey.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gnqeozytp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gjsrnfcnc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gwiiuzlqb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gsblujpgm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gikzjwnxn.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gbsqnrcxq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gxeimcktn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/ggedhfjvg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gqkqqpnez.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gojpidriq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/glxwtlbib.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gthrjhtnp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gsgfpfbrl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/guowdezix.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gsjcfctyq.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gdanuozno.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/geoguyota.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gsrfamujf.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/goeqjodil.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gsjexcrct.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gkvupecjp.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gdiptibtr.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gitfsqhqb.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/grwoychxf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gqayzasbs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gzldmnvbc.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gtrrjtqsp.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gqheiimuc.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gbahfhjhk.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gbfgcgpsp.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/gzabdxvzt.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gkqrkrhlw.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gofecgdqq.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gehhgojyi.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gxfbodybp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gnzsktyhc.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gnnxkwszq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gmpwkxjvm.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gzlxvakkj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gkcywkpys.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gbpyziauh.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gblahroae.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/ghsjihdfk.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gkptaewqk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gxxubxdut.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/geqquseoy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gqgkfywug.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/grxlwjuks.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/ggbrkbldz.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gywhuyecu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/giioajoft.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/ggshdxkjh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gwjtiljhe.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gqncubato.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gndzazwwy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gjfaaezms.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/goodhmdcd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gvyagvzfl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gkhnlalwy.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/glylucsrh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gaoggqvkg.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gmcdaasya.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/guvptlbtc.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gmczxduhn.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gwrfzlobu.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gwzvxngpd.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gcaraskrs.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/glwlyleej.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gvlwapnwz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gcognelmq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gpfwlglfq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gpsdndejq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/guvwkddmg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gevvttghq.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gslqtbpjw.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gxwecfvzl.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gtzyedyud.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gmzttwzsf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/ggynhmkok.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gyologsnl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gcfkzzzxm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/ggnjhiiku.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gkywzrmss.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gxyxmahgx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gzibztrvs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/giwnehkij.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gpcczacgj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gghjizhnz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gckwsnotf.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gcphudpvs.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gnjsbvnna.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gmejhcmrx.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gdydlgirl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/ggvajtuzd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gtzahufdp.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gwikazdbq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/guaiegmqy.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvvyxsoyq.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gepmvqcoz.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gaqghvrlc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gazwprvrc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gtsutkiye.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gbwkqevbh.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gugjrpdyz.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gpmtrqkno.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gzrwgjord.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/glnvahfjc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gutkpkjsy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gkkfnijed.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/ghicdjkje.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gkbsdseka.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gihnmurjo.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gvxouoabw.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gncrkwbys.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/ggmypjneq.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gffqiztld.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghlgwgzjt.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/grsuwxedx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gnjxbmnix.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/ghdxgkyhg.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gcovrqmkp.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gcffvdopk.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gvewujbqh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/gohllrjxq.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gapnnaavu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gclgpjszd.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/ggjkysaro.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gichspmso.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gfblkjvyw.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/grpyrmryo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gnfuhebpc.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gyyxutuhm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gxjmjnqsi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gjujavrpu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/ghjvfkcia.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gquyvluyt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gaqgqrrdx.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gvkwtgwkl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gdrnszaaa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gestjnkcf.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gariiupsi.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gslpymtle.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gqpnpmtsu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gpdnbtlpq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gyfwodzie.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gmxutfvpt.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/gpyoupruf.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gdocrumkj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gakxhygul.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gozxggiau.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gnzolibsy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gpvxtxcnv.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gdpposljo.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/guiitcomw.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gtiwbllrt.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gqkqrundf.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gwdhsokzt.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gzlrcayno.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gycbihsmf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gpgtngmwv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gfwuhrknl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gqgwzkidg.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gyjmodzko.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gglwuzgxk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gdisgyeoc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gqtuvefbd.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gnyygjzsd.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gajucoodd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gdnkmnexo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gclxukorg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gwhkxrwpp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gbvdnuxfh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/ghfxkwezh.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/ggjxjmyjv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gvwgyumsb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gouakdrle.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/ghyzjjayt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gcjasblmr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gzkkqvidf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gcpncdbyi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gpruhvpgb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gktzfswpy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gppmrybwe.sHtML


<!-- 参考信息 -->