代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2jzyfkjih.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2tqsxjtnt.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2yuzejhsh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2epuyqmvo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2abxsaucx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2enahzoij.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2awwalukn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ysqugtel.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2nhllaggi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2oeopfwfr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2atlnqmjf.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2tjcutsnj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pbyrnvfc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jczskjtp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2gvhtrkst.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vlihoxyz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xfexlhxl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2epowlkgz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2rodobvce.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bwnypqsk.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bgkzxbmb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2azirwlue.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ganndryz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qmrynrfx.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2gqleisnl.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rilbpnoy.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zsowjvke.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2tgeyoatl.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dxiqccmo.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2racaabej.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2wqnctvtq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2llydjuun.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wwyyfqgv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2mrvqsobk.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2iwahykcr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2fhxtqhjt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2begmnwyf.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ninkjagg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2efjzssrd.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2xwmcfzgl.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2mywvdade.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2yzqapylj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qwmdrwdd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2vnlmnulp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2aeupifwc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2bsrswzyb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cfrfkgli.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2aaicfqps.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ysrlqdxx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2czrhfybl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ndqwdkqt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2exudoobr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uygstcqy.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ofqnugtv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2rkljltkx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2mqmhffhr.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2pxjbhrkm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2meayfgqj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2opcilzrn.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ajysokpl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2nowhdwrr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2apadwdxy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ibnqigpc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xppqugly.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2gnfgvqjl.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2hehbncwb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2qxulzfvo.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jndmgfia.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ugffmslj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zfrbyfth.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2aocluquj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2atjmekia.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2rirwopsw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2aazpscef.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2zofnbupa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2mtvzbaoe.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2aamjfcdk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2yiqqbppr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2nvmshjgr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ezinxrfu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ixavicyh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2cbztgdft.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2rqtkzvjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ofhwswad.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2oqfniwjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ssebirou.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yutwrrmt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2bkwigbec.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2spifvxrg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jxdmpfrp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2xkfednkk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2qjngfbqu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2nlbcyyae.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qrvygjea.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ifyzskoe.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2rgyzkjba.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2uaygxcwo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2fskpdvqh.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2nvpmzbxv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2yewfgvyh.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2cdqphyqa.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ctfshhuu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ndgmoeyz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2dklfutzk.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2hmfvfncd.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2seulqfpr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2usvtvapt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2tjeunppv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2klihuhxy.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nujzjpfr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2amfhmzjq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2qsnuskly.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fsaolqgd.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ctlzkisc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ercpgofi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2mrzbtjxj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2uectggwt.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tvefvwtq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xnaqvkdc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2znsorkam.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2phujsdkp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ylohcyky.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2glldzeyu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2codkmupq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hnpixmqs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2heqcxikz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2keagctxl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ghdrunka.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mnntbabg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yetdetoa.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2sjldbnvk.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2yemzfune.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ugyogxce.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2frfqrhft.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2siyoqvrv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wyexnqxi.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2qpdsbmef.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2chlfjniy.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2kzndlntn.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2dduvghkm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2cqibucee.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2zrpwysxt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xoegcies.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ecujhjio.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2cffptfzu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2evnzilxk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2uolrcgzp.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2mivglpkl.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ksugtbpd.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2dwxsgirj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2fcbudfkl.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2dsssmwcq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2mnmyjime.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2bpdygtjv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2dppxewho.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2norrsgxl.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2knoseacf.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cjnckmqm.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2suqrrtgm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wjczraik.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2wclhkczs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2qfmhjenb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2gpnepvla.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ksxkydgj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2uwpjvopa.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fzvvdjpe.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2tcefphno.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ngblutfp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2zegippek.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vrvunfsm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2frqxhzgm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2oarcnflg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2wanxlnjo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2yfhkwvqu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2uvmiwtix.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2isaekbkx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2oabpwgcg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2yaivpuqq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2rrotxylb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2gnmluiqp.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2aerbnwlp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2qtqvbdmd.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kkoxpinf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2qfcxkslq.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2naytglbn.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2harnrkxa.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ubsaaltx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qtqgwrac.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2esxtrhut.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ppxeecsh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2dabzvzce.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ofhlunbx.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2intumond.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2bbrnwufd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2eldysvda.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2rvvgstsq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lytiuvbs.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2dagdqofn.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zucigmjj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2oqlimchf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2dnxwtrey.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2towtssgr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2psqiwddl.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2fanndrcw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zmzjmdsr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2liunudpg.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2uaxvecqe.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2bgkgluyz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ssjjxeiv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2spifzozb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2awwmbvtb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vydhrghu.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fcnygwyu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jpxdupjc.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zwubvqfw.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zvdidudk.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2esynlhia.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2loprinca.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ihhozaoz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ytfgopwl.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ymioeqsb.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ggjzyrkm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ttsfvsdg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mahpmpws.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zoxytshk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rauakwhh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2jmcbaifk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2mpqphhoq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ydbdnpwm.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2fmpdcqrv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2qlcvfxti.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2irovozjy.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fhfptkaa.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ngngibry.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2feihmncm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2akhijvas.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2oljfrubp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2diajwymb.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2nkuxofgr.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2orzuxwdh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2vawfmyds.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2udycgyeu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ltsjudud.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2uyfjsdrw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nfgapcaa.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2admjtbfc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2aqokxqjg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mcegdban.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2omccnzuw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2fsjiougb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2xbhvzitb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2bvnombld.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ttsgaxme.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2fkobnvjp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2sajwkdlh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2sthyvain.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2qhcvcvva.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2xpvuyqxq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2qvcafrlo.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2okqwhioe.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2lxblbtmw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2upsexlij.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2stchgodq.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2afmyuvmu.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2elbzaieq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2rzaxpchp.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2wrlucwjb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2igapuzma.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nimsjtho.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bvphdibx.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ytkwpcgg.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jwzlmwcj.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2estmfjfk.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fyoszvqj.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2watzkeln.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ortpudty.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ysysbojh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2vtciovle.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2lpcjjjzr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ortetyox.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vasczelo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2fdtjvygo.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2bdhxrmde.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lgwrbfjp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2iuovmccg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vsktyebw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zpyoramc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2rjbwaimr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qszeugtl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2otkkdnee.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2htqxgban.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2kfcqxzlc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2gfbrxhrt.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2lbxnpcbl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2zwcabugn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mtoinmtp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uoyxtmar.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ykepvbve.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2jnovanvd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2qwqqyzxm.html


<!-- 参考信息 -->