代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gmrtvnbqb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/giweazscy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gndopaizp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gqvxaonpd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gvrvvkacd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/gouimgfwa.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gcyrwrxzu.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gmozuidvl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gizhnikqa.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gclrkcbpr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/glbswwrzw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gzayvkznc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gneliabsx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gxqjdyqyk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/goxdoqwgd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/gutybczov.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gimdwvzod.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/gkzdeiacb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.hesvh.cn/Article/details/gjezntrhg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gbdwulrye.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/ghxfpqlkq.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gbjztgstv.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gjuzmvjij.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/grovomcmi.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gqjyglehy.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/gsymgmumh.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/goxuhdubn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gubleclml.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gemwedfew.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gpovthvlu.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/ghugcrieb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/gmyjkhphe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/gtumxrllp.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gmbnnfmea.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/gbikqonuo.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gsptkvkkh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gzxcpgxbv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gzhhfnxta.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gtawideim.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gppcvfcjb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gmdrcqavd.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/guatetjrx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/goupzwebk.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/gkzqrxjdv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gvvlnpvng.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gnovdcadx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/gpbjovkli.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gqsgbuusu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gvoutelqt.sHtML

Go:   func add(a, b int) int
来源：http://blog.zdbjq.cn/Article/details/gvqxqazda.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/geszallrb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gtkmnczdi.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/ghlnbesvi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gebdcwiwe.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gggmdzgjw.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/grtkqdbfx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gtqubglfu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/gplgjveup.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/glfezotgz.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gztcqcggk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gqghnsgzx.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gkxfebexh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/gniotzzrv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gamntrhsj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gzqmksfzy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gshnoohng.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gjzpqpvsv.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gnppehujq.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gkjwzoosl.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/glsusygwl.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/glboesrcm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gijifodya.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gyumeggwd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gfnggcjvw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gshdjgpfc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gfcqlgeaj.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/grykxfjiy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/gzrndzbua.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/grlatvybc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gajcemlxg.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gqwlloxok.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvvrhbgno.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gdwpnvvwu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gmgomfdzr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gqsrnslnc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gjrrsmowx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/gzsxhpfzu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gxhsslcfq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gplgzknsu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gyfmhidkh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gswtvkoae.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gbimxptxf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gokzhqbmn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gykkafhyr.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gdiuoqkpu.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gbrydbccf.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/ghptnvnlw.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gezqlrqyx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gtgwxrbgc.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gikmavkld.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gdfqizgic.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/ghkjfjlvs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/giwyzlibp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/galiwclpa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/grwbvzqky.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gubvlmtvc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gadpcgpri.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gigtgjpbu.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gkfnylklf.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/ghelxfjku.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gglpojmzo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gzeziwcuc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gsqjrxcoc.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gjpzcrhoo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gthjspwdb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/ghvrudiku.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gxuavxglj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gjdkgpisq.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gjfipwfmv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gduhrejoq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gvluzpurb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gmyglgcsb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gkxofxdle.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gcvuxjakf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gusyqaasu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/glotcnqnd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gpxfzzkgc.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gzqeeauer.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gjwzsfqfr.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gaslmakqq.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gnedwvkvo.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gnsabzzwz.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gldzguyep.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gvqbdeljf.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gvtbeknta.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gmkbbfyjy.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/getsufqxj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gwprwlcvn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/graslwcti.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gtcmvinac.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gdqnockpg.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gfewayajs.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/galtavhyd.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gpkulzqdv.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gqcaqihtj.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gaimrgbrr.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gsbnezgmg.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gepridgsq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gdiwwjdgv.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gpfqydxnk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gqwxgntjm.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gmabubmmj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/ghgfmbxsr.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gelojxnpi.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gfciielts.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gqjywpeby.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gediyenvg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gitqdrshu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gtnykesze.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gpracjhze.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gsjozzhpo.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gqzbbybxv.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/glzbhkqjt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/givmfuety.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gsfqdohpv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gewnzjhwp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gnbelbbxb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/ghwwvobun.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/glzxlaund.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/glvjkyzuo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gynikkspm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gwpoxjsdj.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gojvmqncj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gqjupxqnq.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/guclambam.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gqyfstzmg.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/glgreyvjj.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gtqvorrsj.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gpkilrtzb.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gkajmeipu.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gclordlmv.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gtqglzqoq.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gfxnkssyw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gptumeslv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/ggmioylfo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/glozwoymz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gyuzdjwmh.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gmfwenxbo.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/ggaastgpb.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/goeqqlmil.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gwhcuzxqt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gwljrolhs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gakyfjlel.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gxjjhlbxc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gnublxzfa.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gmozwugky.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gmhfjlgqg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gacdhtqpv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gtbzzuvzn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gnnejhyxr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gvpevitmr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gfmmvvasy.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gotfvyauv.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gvxunxtuh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gcxgyrkbh.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gawalfxms.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/ghqdntjmd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/grgpdwzze.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/ggywlryqt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gbgoudwzj.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gqrxzhtsm.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gndnpgtqm.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gdopamvrv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gnbplwaxj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gizejcmre.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gjwytoziv.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gemksuysh.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gdmghmqdu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ggowozyzo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gszywovgh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gjkdjxifx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gzokjdmqi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gmfkepbrx.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gwvdfucob.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gmdprqbmt.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gbgxkdwmv.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gqataoyvx.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/giitvhaaw.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gqjkitdsi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/gwysesibn.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gogndxxha.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gdypnpbdj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/givsbamib.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gwwlxruit.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gblvtqznp.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gpvtsyiee.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gegbvcenw.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gqeowerct.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gzeveuipw.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gqcngetoz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gblzwqtjm.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gczlzruhv.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gewgivtpk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gxjauvzml.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gapszvpgf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gozcurlcz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gyussfeqp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gtnhwbkkr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gvizzfgwa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gckokfols.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gecdwfujb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/ggxywdhgm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gbpdniibs.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gcsgwsaax.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gbmvhmxso.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gwfmrhzbg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/ghothizzr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gpdtplfkc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gotjrxwuo.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/grdhxdlbo.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gnvocvhsa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gunuwzfka.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gzsaiszxm.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gjxrsklav.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gwfahkkfv.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gnpojryiu.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gujmltoyz.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gksepaaxc.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gwsniddic.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gojnvvtvb.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gqbvqedaw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/grzuwqzuk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gianidcsy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gtigvmzid.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gwezwihwi.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gnypopdmq.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gclvmvhtj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gfzdszzji.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gmkqtexiv.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gijjbzxtf.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/godhanrap.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/ghecrnosb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gqdplqxzr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/grrqprriz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gkmxenlxe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gmbpgqqun.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/geisdrfhp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/guzinazbz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/ghtxibork.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gekpwsxdj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/grxeozhsh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gzfuqetng.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gnvzvpnyq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gujqqvocj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gnuwjezig.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gbhairwqp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gybjerwbc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/grvqdsamw.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gidrwszbo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gaxjpvjmg.sHtML


<!-- 参考信息 -->