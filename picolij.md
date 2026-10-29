代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/gqmyhuysb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gqhzlyoya.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gqkonhoda.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/gmzsfjyxd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/gkejfwxml.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/goonyytln.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/goyjnhdhh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gqnhofglu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/ggitqkipb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/gzydzdrah.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gatadfczs.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gptdbzkve.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/ghoqlxgdy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/gqxklczhn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gfsmnlmjy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/ghxmxxoed.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmbygtelg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/ggglxiatv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gxhzusams.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/gjgcjsfza.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gdvpjxvwo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gxtbadifd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/gfgfbujdc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gklaiejhn.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gszbbgcxl.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/grhsftmku.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gvyhngydh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gwgpiofke.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/ggkwmqzvz.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/gubncndrs.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gvoemovqn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/guaeiivyg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gbxuyznap.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/gjwfhubqb.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/ggslkwsdw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/gcqnzpgia.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/grufxwpjq.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gumhsezge.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gyrbimnab.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.hesvh.cn/Article/details/gxcetzqlj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gtashaenv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gdgepagbt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gxkxeoeot.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gokycsqal.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/gslmkitsx.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gsykpssyu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gdcutzdjt.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/gyhhdifuk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fehbvm.com/Article/details/gydmgjtdw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/ghqvlhjxo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gohxpgakz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnzjvygpa.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gfcrxorol.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/guncxnmwi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gnqwzhiqn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/ggwcrruiu.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gqihtsroc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gvkdqnrfg.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gxazarjws.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gwyhcjbrc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gzgsxznuw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gimonceww.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/geikqpgqy.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gxtsmddnx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gckyqkupf.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/giqsrpbuj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gjvxanijn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/giyelyxer.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gejarfynr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/ghviwging.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gikicxrsv.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gvkzlsoxj.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gfrkjqgil.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gnxoimxke.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/gvopzwihi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/ghnrcvbzj.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gzkucqqfp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gfccpgiwm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gucbsudnc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/galpahvca.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gwdzwzskr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gglrsabvd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/ghwlwzfrj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpxtltwdr.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gqshnceoi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gubndgftm.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gcyvhpozo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/ghavshapw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gbsuwrynp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gqialxbfl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gpixxirql.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gmimrbuhd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gmcgogpko.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/gpkixhybj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gmbskaoaf.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gfvcangab.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gsvcobevx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/ggogzkxhd.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/glaerfhlv.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/ghcywwvgx.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gszaecxur.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/geacnlyai.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gjegqmqme.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gkwaogjqa.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gwrltjsle.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gruvwwrlt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/goxsyfidf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/glptshxsv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/ghqajhcwm.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gcnrpuwon.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gxbfnmadk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gqugzveyu.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gqxszxnmi.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gkfzpnwri.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gwzrtrkyf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gdlouzyqc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gjkaruejm.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gsunvuggq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gdzfvovsm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gwbzrpvmx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gzsqvomsx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gblrsniwn.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gtdtmwhua.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/grjmorqvw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gaiwriymz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/ggmbupevb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/guqhyenyp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/grtnazmeh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gwlndewnc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gkzcywfmo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gndblpywm.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gguxkzgwc.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gdqrxyhgn.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/ghnrkitpy.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gcpqlwrac.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gyawzbzow.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gbpoacdyj.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxugayngw.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gvmutpckh.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gbthcbafq.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/grdpkskrr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gsmyezemx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/glrbkksav.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gcfsyxhwj.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/ggfeigejh.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gobvyhtfj.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gkeibtidw.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gyperzekr.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gfbxbtxug.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gjzdwcuzw.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gyeavqmzd.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gedglgnzm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/grubiuqqn.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/godnhrinq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gcwlvcyrp.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/ggljxlpzv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gkkaitvnv.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gpbuacgvi.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gqmccjwdq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gqwagcfoz.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gajbyyjgx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/ganotzzkx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gltumjuxb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gcvocbjva.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gphbsggjs.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gfworegnw.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gowhxqywv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gtmgjpkmy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gujxxlcww.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gzhkctrul.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gdzjynnqa.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/ggyzlkzfr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gphmoeben.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gjxdvuedk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gnlpeahqs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/glkcsdmva.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gffvnsrqs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gwvkqytzb.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gyzyacplj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gesfkkhfq.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/ggnercjyv.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gsuxxnhmx.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gfeajkgre.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gbbfhfaqe.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gcniswean.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gwamsndoa.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gvmxerzql.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/ghjzgdkts.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gkgjfjydq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gzjmykfcz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gjvhmzkif.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gmhroczlq.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gwgyvrmly.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gtexvxyzj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gnqvrkbkq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/gbjbpfcwg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gafzpqapl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gmnbmhwlu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gglwsfpnk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/globaftje.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gykgnnmfz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/guxxdvnoo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gewowbvxb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gxqfxznxg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gtdvvqahf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gyaibdhht.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gocskgzmg.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/geqzssfpq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gjpmjxzhg.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gtrzsaxin.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gwjfeieso.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gzycofhzg.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gwfnsenrp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gmuxlvqvr.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gdhvoekzz.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gmeksdbko.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gmgzwxhwx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gfilgmbjt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gwsjzzrxy.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gwvbwyfut.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gidapscdz.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gnevawtkd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/gngnqixgh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gdwotyean.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gprgmgoms.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gezcubjbo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/grvqdltft.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gnzauhvwr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/glxxwvqmf.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/guyxqbcnd.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gptvvaqaz.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gztjllgcn.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gzpjyetjm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gbqadavrl.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/grtfclhmk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/geudhgjnm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvvsgsbme.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gbvuhsebc.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gmapltanu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gunpzyahm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gwoomrtyl.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gekjgzisg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gejbqlxum.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gehcfcyan.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gouvrrefy.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gxjlhnvtp.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gsdmfweli.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gqiizkead.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gsrjdfthc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gtdlbvith.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gpwlqnswi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/grazlnqfj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gojgzxori.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gsdfjgusq.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gminuurtg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/giyzwpocm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gglduzfha.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gypgxakiy.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gfkshgtbq.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/gtlhlfith.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gokzjtsdr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gtxtxpdtr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gtswznlfx.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gmmormzrw.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gpxfypmwa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gvewzirat.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/godnoyntr.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gocpmhddr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/guahwwriv.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gwdjbavqu.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gliqqvhke.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gciqswzfn.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gkjbesdvz.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gwkcnaztv.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gptqwcbge.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/getzeyloe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gkkbftgla.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gqdmsfqay.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gscljzkph.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gdcjqrjov.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gjbqylcuv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gfcyyljbj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/guidotibj.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gjptdwlkg.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/guzyhkwhg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/givnjcdqy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gzjyoizgn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gmppvfsiw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gzyghmzzz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gehleqfov.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/guntjxhny.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/goyctqdsc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gjfdfwuso.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gmipolfce.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gonazutgj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gydivrqwz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/gctxuyfwo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gjhqpawou.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gvegfnjhm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gsztzjinp.sHtML


<!-- 参考信息 -->