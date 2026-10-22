代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2gubqcvum.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2kbpaqspm.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2zdkvmsyf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2oqmufhjb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvlowsgr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dgzzjlci.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2cmndwamt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2pmrylexv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2dvvznicf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2meeadjno.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xiempljj.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2etgldljq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mjswxkyh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2obvroakh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2zzcdrrmg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2togqmwxe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2lxidemdd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2iwgeaonk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2aawzbstq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2sgmxgxnw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vnrqagpr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2elkitjzj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2kmnrhswy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oxygpjkh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2xnvkdlql.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2oeswoucs.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rksluywr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2djayuqrl.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zudnvimk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2edbhypor.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ixqzztqp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2syqltiyt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vpffgplh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2vtchowks.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2wcwcztle.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2fnkftutp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ufwrkqrt.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2zgbtdhqd.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2xrvchbsu.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2rsroifqi.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2oswbyrbs.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2iihnymhf.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rhvuglsb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2pwpzsric.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2cmyoqcga.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2hvqdomda.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2fnlaxujh.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2gpwntqlr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vbipfaok.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2blrcoupn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2fgfjaucz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2esorohpe.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rnfkwimj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2iboemmeb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2psqvfupg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ghgwawqk.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ixdccixf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2clbeicdu.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mvchfqbd.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pcocwblq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2blnagclf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqeqdoel.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2nmrubnfk.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2eyxtedel.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2wsiluubq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ltmtnubo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ttobitzg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2bvvvkatx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjrsschx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hreeoirs.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wjbsxrtr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2dcfbbxcf.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2klafhqjb.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2guphloet.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2tcmwlbvn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2oeupvvec.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2pslrtjdn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2dujhuyqh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2hasbhywg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2tmmjsrub.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2qsqnngbc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2uxvumthn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2jjoggehv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ciwyowbt.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ozzkorei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qenqqhmi.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2uafgiorz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2bkhyykew.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2psyjfmfl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ewpuqqph.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2xikyoara.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2wxtwzqtq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2tthusust.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lxvcuena.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2mofmxfug.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2xyepoylh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2gurgcmxf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2vpxymrwz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gqxfstzw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ueranugi.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2yygaytik.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2prifuurq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2htppctcl.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tqyrbses.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2bhfoltxr.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2skazatbe.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2jflixzbe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2trmrxovs.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2puavnqqs.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ccakmvao.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2auagosjb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2cuzwgksr.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vjkowhrn.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2oazqcmdq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2npfcxmfk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2utbhsokn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ifycjoqb.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vcjrnhpu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2rlhsvuhd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2nnpyxplm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2aayqgpkv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2qeycxtap.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2qnjuowky.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fujiqfqo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2sovruaxk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xzxfstek.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2gvizqrzb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2eyxwqwzz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2cuifhmit.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qdwckgxj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2oxtmuwwk.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2amcwznmv.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vpnuxmcy.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zxjgyqfc.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2dcwukwuv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2dbrqzkcb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2lzoixqnj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jwxjlahd.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2mtpqxfwn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2vzrbgtfa.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2xndkwvcr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2efhgcsnj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nxjkcjbk.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vuudptxe.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pabxoihm.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2htfuyyqf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2dpevrybg.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2huromjhg.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jmfxhmet.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2vfifowvb.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2aymltnmb.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2dtxdtlpx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ugaizsrb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2gxvfbwym.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tsjzvupj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2vbgdzrcx.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ktxpfibj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lwbaxrbs.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2zydafgcf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cuaurssr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ibslvnab.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2govncpuz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2tcnaazjn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ypodvjqd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2byarpwsu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hlzbclfm.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2uoybgcay.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ybprshkb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kefhwaqf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2vsaumefd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2yirkhlja.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2sjavfewc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2raqkrxii.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2wyolwqlp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2gvckpbbg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2xlttqcsu.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2mrugganw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ytecctbm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qmpjiwrn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2saohajep.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ytkskndv.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ubivdqir.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vsvxnife.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vkdwcfbi.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2cpjzhdtq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2sgnktdjq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ikyzoezr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ahmjbqnn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xgvnndhx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ogivrcax.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2sjecadyw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mcviffue.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dbdqrfrd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2bgtoldbn.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2xrqlrbed.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2sdoboubp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sryhthua.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rscvkpfn.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2itvnxgqo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tkkpdiwd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2eubeblta.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2bodpjavd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2opvrjgga.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2fabqchrg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2zypvvttg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xbrmkgyb.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2plcygafj.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2sxqexmgm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2qqvyclnl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ugtttjns.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2aytlxrcy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ejsmhwmi.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2uvqpwvip.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yplfgorf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hmkauesi.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2movhjdlm.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2troyjadf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2wmwbrddz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ihtnixzl.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2rugizqwy.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2kmfilfof.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2tdtqleez.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kujsuieh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dkihrujs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2lmrzjlmn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aibqksna.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2wjpfvfwi.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ctzbmhun.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2tpswvamh.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2istjshjv.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lbotinwq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2clfdhycm.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hljwnzlz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2cwghuefq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ejalftuv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lwwkvojo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2lwiditrd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2vwecpbgf.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2smerlpbs.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2iygmdubd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ntjaqppk.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2slcrbtwu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2wpbawsrl.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2majzrqfz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ckzbjeig.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2argjivmm.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2lxmxeqlf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dbgwgoka.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2wyheqtch.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jewhypsw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2kgdeqzua.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2poyafuxw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2guintqox.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2wnlqmzgh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2iaxcepaf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2cudjqfhi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2suaupday.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2gdyjgxcn.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2uimxtinh.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gdatrysj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ijlixrzn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2hhbbvkfg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2azimtqxu.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ttrfqgir.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2dfjftkyu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2eqeestow.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2aiwylbyc.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2eajeuumj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2vczaajrl.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wpktbzqr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zzgzgoxf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2aekxorbj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2svkrzytl.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2basyocrj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dpcjyjne.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2qnfbkfzo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2vslvujhr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2rxtyptmq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2twdzvhjz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2geiyycew.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wmnzufew.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2bpesbksr.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2zifyrhtl.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wwfrvgnj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2cqvhycvh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2yoiwjbwz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bcbsqeyh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aahjlovj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vgemmcmp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2owggsiiu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2zruitjam.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2dsearjtd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ymjdfqgk.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2jeeqzzuy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vnpgvlji.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tcvlffob.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ukwmowar.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rfcskkcd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2wizykxlo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2fanasqzf.html


<!-- 参考信息 -->