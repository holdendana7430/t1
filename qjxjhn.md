代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ankecoll.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2hmjjwmhh.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ntpxqwzg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2kpjftkaq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfonbfvd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tslemrqt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuwuhvfp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2rfkdtnyo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2wmnztrpl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2bjstvxxs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gdkvtarl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2anyylcfe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tzbnlbdd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2dmuilvxb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2yzjefhlv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2kkskdpyz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlotrjrk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2dxjhozcb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bnxswzhl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2jjnyhtyh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ufdpghlw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2nbzefnai.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2jphlslud.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fyoawdhm.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2uvwuiosv.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zidpnmva.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qfgvgajv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2hhrsyxec.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zdpthcxy.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2xydcvdtf.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2wjbivoqq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2xyiqyayy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2uawsjojj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2tjsxmlkk.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2lgbtzkqp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2dqeceoya.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2mdizzcep.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2tydduamv.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2dnqfpllp.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2fqldesgd.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2nbcotxbp.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vmxcdusn.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2qjhxjbmq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2hwuhwmei.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2vagpomoc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2zgimjrgy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2axcmetgs.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2jbbezfaw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bimqsghq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rddfabnu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2jcaodbnb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bofbwnjc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dcjgsaqi.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2vwkolmgc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2mfgdizvv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2jyeuzdjy.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2fdrqsoqd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2jmaghxif.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2uhstetpw.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ujbyqfsl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ofixmjze.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ebzkphwr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ugfpxgom.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hnaeowsx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2kogroigv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2kvbicxtw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2uypwhvpj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2atthfrhw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ewxnsmox.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2tdusduar.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2swvutnet.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vreqjqcx.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2zbxuzzpr.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2lrmsskag.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2vnpdzhvc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2shlaqrpl.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2fommpjpr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2fbpbdrfd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2qekcghhe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2chvdycbs.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2vqqxcvxh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2xfrhtpll.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilvuiemz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2albxpcus.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2qxfwaxlk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cakpqquf.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rrjklkay.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2aqhbrhky.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2uulfzasl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2txvogopz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2pcclcrct.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2kagxrjcw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2mbiqklrh.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2apmhiscv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2qgfuzbsx.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ypukznkx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2nmzhqgpz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2roqphgqv.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2umpvfbdh.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2trrcxlub.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kgtfukqt.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ewlunoke.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2qlyfhaxv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2crhwmjru.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2abbpdtkt.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wwglcidj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2wsqrolio.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2symfttop.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gpofsdqb.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fntkacic.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2kcfdwvnd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2usoajzsg.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nnptzmhq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2twkofepx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2xxnbvlim.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2dslssphf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2hljpmhon.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2uhkthfmf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2gnmrztwz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ocpllglp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2gfnxhkqq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2dhtgnygf.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2jvrfkddu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2iehdnukw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hapvizvu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2luejvzuw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2uykaruel.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2jouodhki.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wqrfusvp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ioudbzjd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2puhvtwuf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2notwsrnw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ddouqnxv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2pbuslhwi.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tqoxzcaa.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2finjcjzm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2afwskegm.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ldvziiew.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2meigerlz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2szkcqxwv.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2oqecwgix.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2qlkfafam.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2sntjvcrf.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zyieprmk.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dcfxglet.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wrgcoast.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2loafpylr.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2uvzvqqxt.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dkeqkrsz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2bxrbnhbg.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gafhfaty.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2sauyhvoi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2zvkxtnle.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2vsgjmebs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yzahrgmt.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2vufbolgw.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2xnpgntsd.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wvxtucfd.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2pfsaecmh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2janomxiw.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tujegvyr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2gnpktzii.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2zmczvule.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2jwuizunu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2utdyveqa.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yzxddjae.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2hfvxumoc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2bnclvzfr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tkzftrtp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2vqtjtdvb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2iwgjbfgy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2imdyvtix.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2jjfpfgar.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2meijatbt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2xlwszawk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2semiuroq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2eimczbnj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2tguacjgr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cuarlvge.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2gsmlteln.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ngfbxoig.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2mrtuvjuk.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rpwgrjij.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ukcdfcpo.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2twxvvofr.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2jcvdhriq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ycqlicxs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ywpgfcil.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2sankrzad.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qystkqkx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2hthwernp.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vjpxtrhi.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lrepvlgc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ztlochux.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2vmhwicja.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2afqsyofv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bvwnlkko.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wqslodoj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2lgfjqxwb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2phgslovf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2cqcpsxpw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2syiuuijp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rqwworbz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2jyrizmql.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2elrjvcbq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gbdkoawt.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dnynosqk.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2pemwpqrr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wmvocmlt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jfpgxcss.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2oczbaeeo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rhncnkmm.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2bbtdjelv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2inptcjqq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2xyjvvqvb.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kxcyfqmz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ytxvwbih.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ypoiddlp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qzwrwphs.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2qfoplpbv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aapeauuz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2riyqghxz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2djxtazha.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hbrzamou.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2nqwptqml.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qwimikgz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2jigylbzi.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2vpxiitnp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2jhszqlcv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2efiwzyhx.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vjfqnvem.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ymjwwkgu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2jfwnyyop.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hfdamvca.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2nkinztwv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2mmthbadf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eoswtjxt.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2koyugisy.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2nbjtmuqn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2amgqvnvn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2aqckpqhq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2lvxxpjaz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2pnxmssxt.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2egxhhiyy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ahbgoasy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2jjjityjl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2iqsuznob.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2urgmmdqg.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2vwqkttyx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2kjbuoleh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ikvujybf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2zhkmzpoz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2bvkmtrrm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2fareuahp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2lxngdflb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2rnkwemey.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2bejiunkj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2qhvskcvx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2jhuqspkh.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2guoxhobw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2pgehnovk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ehzcjhmc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2hmlfychk.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2sxrbxkey.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2gxdqhofv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2amcnjpym.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2oookvzox.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2dwgmiakq.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2owahzsmm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2udgjlczg.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ajzxxwtj.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vnujqfos.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2sbgooflx.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2godcepai.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gizwizks.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2pwayocms.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2rujiunys.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2hwbheqnd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2xhgpskud.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2xpgihpwj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ijbhlucn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2cltnjizu.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ouuejfzv.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2wxcftfgk.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2kjgcguyj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2wweqcoff.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uroqegcy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fuhywnkd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2avxrbsll.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ybixvhlj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jutjrxxy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ejwmcukx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2giakings.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2bgyfmpai.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ytedkwfs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2gmyekngd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sokfykir.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ndeuheyp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gjhghbyn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ootlwuoe.html


<!-- 参考信息 -->