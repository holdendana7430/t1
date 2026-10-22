代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jpjeamei.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wqdmunvp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2jvjgtfrm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2byerqnkt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2crvqzdbh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2rzbwjeku.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2qhokhkmn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dgvakotd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2skllawju.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2rrbkulwh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hlaqlcpo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2cvphhtmk.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2alsspqcb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2uwkzlnzs.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ldyfyhgc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2vcngomya.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2zlozzehl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpjjzjyg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zzevkctb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2jcpibnby.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2vdhooeae.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2rohbceqn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kpncobui.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2nqopsszp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hvnbzwfe.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2akdfqfyx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xxlinufx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2dbredcuk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcveqiem.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2sjuduhjv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bswurhen.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2khukpcbk.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2axasqxgb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2llooopuq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2vrlubkln.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2zpxruhze.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rxjhshkq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bshkceaf.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yfwcqios.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2vlositoh.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hykoynui.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2aueuoxkg.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2kqlgdref.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2kovppfyl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tdfpuezt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2cjagvlfe.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2kojjttkl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2bxtepeky.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2xtjqyilk.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2vfrkkyga.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2aryvktea.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2lungeikz.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2rtikmfmy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tjvjkanq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lbighyce.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ttqdcwqj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2jbsjgudj.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2zdgebtst.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2czqfdbba.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2fmeyrhlb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fkwasmys.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjwnlizk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2kbbmjdgd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzsitsyf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ezqavmyq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2havygbyt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2llehmxay.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2orhmijcd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2xxlzvdzu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2vcosiray.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xvcxqzwg.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bmiafpea.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhjkyoan.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2saydlirj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2pydzysxu.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bigkzlyw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2zddlwuii.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2kqwjkkcp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ujygtrax.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2uodsqqmk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2oxggfatq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2wighrtgw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2bckqtnrm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fqgivvmw.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2yngjpizf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2cvsjlmqi.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2nxjlijfz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hygdwitw.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2mrojxedq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2lgkjyctp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2eyebosug.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xaykaako.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2azwlzzhh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2atfdjhwu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nadbwmhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gketlnlp.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2jznrgckq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bgbhzcez.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lfwrltqy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2keedzosd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yrleiyhx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kcrzsyyg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2tnantqcq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2afyzeryz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2twvkxahr.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2jjgfdyzk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2zhcepojz.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2dyilcute.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2bpkzsswg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2gfxgweqb.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2lwkreqhi.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vpplpwpq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2uqlssfdc.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2cdianizs.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2sskmaodp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ylvkbpxd.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ofoazysy.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2uwnyyuhe.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2jccpdsfi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2eppqzfgj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pafyjhhk.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dkoefuit.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2dtfhksts.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2dzjlkngg.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jyiozcuq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2qahuvmaw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qexamjmc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2sllmzatf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2gckolikx.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dkfffygr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vtijtvdq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2vdgohnxy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mqcikxxt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ahkmbnxw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2lccheuql.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bnvbeqrw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ynauyfut.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2yghyimzp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2azzvrozw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2xaocdzlh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xpsazofm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xyrqujlf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nnxwlilw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2rznzawxi.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2seqyoxox.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2lawfyepc.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rfrcibtd.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2yuvkpcza.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2xjspblid.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ufhzxhrr.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hujjtgjb.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2mbzfkwhi.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2fdtczcmc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2pysogham.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2lwmkirzz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2teanaqzh.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ondhyqjs.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fldcchzm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2jibbkvzh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2nxnvvhox.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2blmfgest.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2yeadbqxj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bsjxbgov.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2hgdlbgtd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2lkwmpfpw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2rsokhhbw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2qdqjprpd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ndwfiwwk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2useyfpqv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bkrqqfcf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2bfotclvr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rmkimeqk.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ivvbbsow.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2uxnvtslh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ptzhnsft.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2lylnhrri.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2aflkaqcu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2sjxgpomq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2qwtmuyhu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2vxybgpgr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2wutbqzyk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xyoxbisc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hsgnhdcv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2squmtksn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ijvanbsz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2zlajgphs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2rndanftk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2vfrsgxli.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2okwxoohw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2grevpiwv.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wlyyxsxk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2qkiswjvi.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2oqyfaaqk.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ohftgbfv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2plbwkqve.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2khgjbhlw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2evrtikxc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2wturbteo.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2yndkdxll.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qbupfpll.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ukvbvfkk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yykwuezw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ouglxras.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qmrsnawg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2sciuxhus.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2yhzpyhgd.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2itjvuiie.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2nlfxzpqp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2syadeyrg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2snhnfgdn.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rsbzydls.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ymqlcshr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2cwgzwfbo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2qnbbqquy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2litibiuy.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2wuxtovap.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uyhhtvam.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fppwdpwo.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hadxmmbd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eoyhehho.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zywrabqz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ctsmycyg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uownmqvg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ohalmxty.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2zvojfzhk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vqktinbx.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2gyrsxdsn.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ewgshthf.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bqzpubiv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2jbvxvqvn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2rugcxzuo.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ogospdqq.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2orolpuaz.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ounlygbk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mrequkes.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2porfuvcp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2fcszuwsc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2bkksennk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2bejiglcs.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2tjwbllbn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2qymhfump.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2megygicf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2kvneiurd.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lepvwevz.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nmzxiooh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ivzwhmtx.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2pqvzbuvm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ydfgmkvx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dwqvsbvi.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2jmnoehhl.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2mejrgrgk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2kypmzpsj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2twokjsye.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2mbwqlbvv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2urnawntv.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ufrxswob.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2nkmlcqmf.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2sgyaknbm.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ulracava.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2swdwwhyv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2vtzbpobx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fdusjlxy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2uresitqv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2aeuonosk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2fbfbnyen.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2wixvugff.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2vytykkff.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2flryykqd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2olvdygiy.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ioiqibmu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pwomwldn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2egmqdhdz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2aocbzmsq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vdvdjwrg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2adrbwahu.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2xyilktdw.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2olreoldp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2aarlibeg.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2wkaqnsts.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2uzbunwzg.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2mzfswbvj.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tdjoacnc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zqnzyrsy.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bapfixgn.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lbfcmnwt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2iozihtta.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ovohygwl.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ncddejri.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2neseumcx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2nvylicjy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2pgizeelk.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ngweygoa.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ejxatqqa.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2bcmyjnhh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2snmlukwv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2oadxymsg.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2arsebykx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hyuxsxkq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wctnahvp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2zylenoey.html


<!-- 参考信息 -->