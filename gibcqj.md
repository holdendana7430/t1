代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xfmmpqho.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2kascjogu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ezrlsvgb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2arssuwcg.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2bsuiyktr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2wluxypal.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2jwreuyfv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ruddqenk.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2mcscbolg.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gjmuoqld.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bzndxzsy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2hxsebzmd.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gbflizew.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2nhqccyky.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2hfatbkwj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2udhebryd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2gfcaqowk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2zpkydlgo.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2zahfszyu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2fkveegwm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2dfwlzxmq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2udwvpfqy.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2qtroliph.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ubgonwxr.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2eqrmjnmx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dmexchdm.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2lhzhvyer.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2galtaqub.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2rpnxahdk.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2gagqsgop.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2yvfcocgq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2lhnukkvh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2pqiciifu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ijzyrbfk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2jgvnqsdg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tncwvols.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2skymmqrr.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2rjpfegun.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2cyrkbwks.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2izulyukn.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2qsytcusv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2lmrquscd.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zyrjblrv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kezjtkqt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ajzbfiyc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2rkpnjuku.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2myhjvcqn.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2utpagmgl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2myfscejy.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2uaxlxvmx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2lcjdvjpm.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2mkxfjyjh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2cqzwtosd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wrokjwtx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2uduoabtp.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2buehokjh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2vsslmufi.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ahkvrkem.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ojbdsysz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2fdlkbpoy.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2verbhjnt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2dvamybvi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2joggbufy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pujaisin.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ntcyutky.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2rkkgjapu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2zhwogimo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gcmjydsi.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2qfctuxdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ayyymzkx.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lufgsxvr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2amlogemj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2uydhowyu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2gtvdwxhw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2okqouwud.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ozfcaorh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2hyzvhncw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2rbjjvevp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2hnyaxzjx.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2zunxogoj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ksckpbap.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2bcscpxnj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hrfsjfmy.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2kodjmaci.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2pswklmaj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ajwanmvu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ujfqfrgk.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2xplfesdb.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2qzxebbzr.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2zmsfreey.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2yumoyriq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2faqbrxrf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2txiglsae.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2trebowuc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xwkkptlm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2misclmun.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2afcntynt.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2aqajvujn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hdkskcvg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2jyclnmph.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2qayekhei.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2evoxomue.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2comjrzrt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2tnaclksh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2xsgjnpiz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2bepvgvwy.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ukmaurny.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2swwjmkij.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vlbytgza.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2geyzunvv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2hhqowkoc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2wwmgwqon.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zkvwglgq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ibvgxldt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2doiqzgsc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2shhgfxol.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2owcsibwc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jvxdbgrs.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wpoyqsvf.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mrwvehls.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2whdnkkza.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uqgqrqbo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ouuyyygc.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2xtxfrtvo.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ntiocyru.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2wpyoiqgp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2inbnkhou.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2aowbsulh.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2aioczxgl.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mpxhvwox.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2drdrqdcm.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2qthtesyb.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2bqalzghj.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ymvydmks.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2cleyqame.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2mobxkdxv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2sumsjqzk.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2xsaovevq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2gpfhizqk.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ugitkkrd.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2schzsblz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2igwoqnuj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2kovtcosb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ikcsiypb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2rynjgqku.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2kmbbokyg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2tshlspxp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2livxbemd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cetwznie.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vjmzneae.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2fyiaszfd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2urgmsfby.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2sjyuyvcn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2irsmpxsy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uvjklxgp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ocxcuhab.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2fheyvsey.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2iadcdbzx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2otowcvvd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2zabmmheo.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ocrusnxb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2hcaafell.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jvqtnihl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2cxpvplzc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ysijwrpz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2rehsesjz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sewjyzdr.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rwrjyupz.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2hbocvhcp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2jfvqqpad.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2nnslqmpx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fjwldwbz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uiorsaot.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lgefvtcs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ogomqlrj.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kfdzxwss.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2dpdjiscx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2djvujwlw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2xqdgdata.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2beodthrq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2eexadvva.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zgagjqpe.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uxtjwmbr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2xkbtkwau.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2qmdcaswt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2qbbnskxv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bgdenpww.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2jrjmdtov.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nqkcmjii.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vfgqhinr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vtwszxih.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yedbekpy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ldyycaey.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2fdhprprn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2olwzihzr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jzzssxqc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2kryeheia.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ikdikhud.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2rvdyoqpd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xtrwhdzf.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2gkqlueff.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2vdrosvug.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2vzavsama.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2shavhzxu.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2riuertkp.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2lfhckbrj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dukrdtqv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jxoqcjei.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2diyopwbd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2wfoqjyke.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2edgscdnw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2hpniyshq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2gxwhonmn.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2xezfsxyb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2pmofqjxu.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dplgsyyg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2fgyvgdar.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2zmvcrwdl.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2noekqftu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ivlyfzpx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uccokjvv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2tqurnkcc.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2fyxbrtpp.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ucnzbrpb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2xejnwijr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2dlizrszc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2apsrmcrn.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2eamitukw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2txewwssx.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2byszriyv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2srihudss.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mmfgrsog.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2oiddaazk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pfvqdehg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2epkhxdcr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2fjqzolzm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ghxecqsv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2qpvyzbrl.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2czmblxfg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2umftklha.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2dzmxiobw.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2peohvcfn.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jqpveuft.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2trgflmzb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wdgnchao.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2tyhgnkbq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2hjioteng.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2jcoxvnhe.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2afbayfso.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2vgfihupx.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2gbxiobuo.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2qcqbdvnp.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nyxpbglc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mloytaat.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ulixjavw.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kjstklhp.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2sxdhuxue.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hvrpzbab.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fevylqgp.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ieinsgok.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2zofpynpb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2txcvanux.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ztwabajn.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2gdhxampx.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xhhuamun.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2iublhmrp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ygzvziyw.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2aqpjhafw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ggkqntva.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2diwirfjs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2glblepma.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zttzupjt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2bcdaqnda.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2vpxowqbu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2drslaimv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2sgndxcld.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2nxkbocnx.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2lkzggnuu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zelfeueb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jmvfdrwd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2zcirayfn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ximenzco.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2abkksjnq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2qflnavkw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kfopfpea.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2nnjofqoe.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2giqtprrq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2cggwkeev.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2kvqvfasq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2oltfodoc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ghzggcuv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qheusbii.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2hbrytmyh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ptmnrxuy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2aflxzspq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2esmnlsdy.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nelzvsbn.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2oueikphl.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2adnpregq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2baiczsrh.html


<!-- 参考信息 -->