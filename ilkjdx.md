代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3kohmgbsw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3qmznnvan.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3cxibrfjf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ciulkbnw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3umyqjtmf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkdmoclr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhbslsps.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3hnkqqbby.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3izdczxfx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3mvncbwtj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gjlwcheq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3uywssxir.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3nkzmpdlh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ghpdgfor.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3aygovpzy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3myyxfwfc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3vialagll.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3vgjakofu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3morwgnik.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ccakvpzz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3efzjxsqm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3eiytqnjz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ztmjhvyh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hqscrzsg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ekctvouq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gflbdxot.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ngawqvtw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3mjuxoper.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fokysree.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ftofucxy.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3kwhmscbw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3izahcnsw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3azxrkprs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3vhyripjn.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3qhhxdbeb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3wlvnhwep.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3dtpnhcxe.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3tamtsabm.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3fwbzzmfg.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3qcuomngu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3yrpzsxqf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ddmellcd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3linqtyca.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3fkrvtfdy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3xkwaqtns.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3wkjntpuz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3iaiietqf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3byttqhoc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mhbyukje.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpyxjiqa.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3jzodmokj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jxnztfbo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zventnnk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3wvdeaeho.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3uhvbieiz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3zyggvceh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3gyzptxgu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3fmrikwjl.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nmqzgori.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ykkaqdyu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3suywkffw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3oaaqrodw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3drnlfxfy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zphsuosr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3fupxyswv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3mkudfosp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ajtuvbjk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3sdswqfpe.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3byxeygwv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3howuqttv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ybugspjv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3capnwoxt.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3igsqnxhd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3qqxfcfze.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3uwxzqvlh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hwaykwaq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3rwvtsgrp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3jdjbbspy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ulmncwbl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjmcawkb.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3bzdweaag.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3uplpitsl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3roybpeja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pyfvzvpi.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ljkawhvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pyqkhrys.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3uwyojdgf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3vqhqdvpw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3znpwegve.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3tyayvyif.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3etwdzgau.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3egvczbud.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3zgkkvnoc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3dwugcfsa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3nyhirckw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3zmwebhxt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3rdxefrck.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ofuhvaop.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3egeekcdn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rbhuwrmv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kqtkidrh.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3znifdbep.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3agkuzzhq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ncwzruvi.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3oczvhznn.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rynseaaj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3srthomyz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3opozfmkg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kmjjjujo.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3auqujuyt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3bsctjjpy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3lnqvjbpi.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gnjcvocp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3fkprpszk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3hlxrhtph.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3rfdsjble.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3rdosbvtc.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3aafrywhl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rscyhfcw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3cgoveqwz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ejuclkev.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3udjrlfkj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3vfehswqi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tpaugpcz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3keqxasvb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3buvhmvqf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3jxfulgtp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3jqzrnzkw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bmlqjvee.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ygjplrdk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ezxatdgx.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ietynors.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bqfmvpex.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jplrnzti.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jkemzpjd.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mczxghez.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3jttabvsh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3isjlxppn.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3fecmtjob.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ywnzfjws.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3yfsgbllw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3fkpdrcja.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ivpalesz.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ufzmhyvr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pdurtybe.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lmeqzejb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3zkrhryce.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3xvonmcla.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ehfyrsgy.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3sqkfnrqz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3znnyxvhn.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3fmhzoxez.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3clfffmue.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ubdyyait.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3davlxvkn.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ujoscsvy.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3kojepamo.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3buxpmkgx.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3oxquatqc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ylovbjzc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ljdpmpjy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3dmzbzmks.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3syslfaog.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3fzrdkuwt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vmbiiwpj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fijwtduf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3lxsgenio.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3huyipwln.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3nkbqfsmr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vminjnoy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cndnamrv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bqqebmlx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3iqozmgkh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3yrybmdic.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3vwcmkxpt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3aeneubyz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ytyhqmce.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3bzowyjdg.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rmveckpg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3mdvrvapx.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3eehnmqif.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hcrgpqwv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pcjpingy.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3edzehcpy.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3gsaqygxh.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3bqyviapt.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qcizhrcp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nnwkseev.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fbudmfpp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ltpdcjuk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3cbaqjaqv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tnpctjbh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3qwgncqoc.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ubaftzcr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3arldhzff.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xempkbye.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3bqxebebx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mqnrjpet.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3itvwnnzs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3sjsiuzsg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3sbqyontc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3akmdpprl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uksrruwu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3iwzjjvuc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yniyqrai.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3biejxivh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wnmooqji.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3saffbnng.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ifauvzbs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ksofvtzy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vjtsfrtd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3virqtshu.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xyvokiwq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3afoxflax.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vticxrlg.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xolfvriq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fkbswbeo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3aozgshwi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3mbzbyszo.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3onzpedrx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hvqrllez.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3chjvnzuh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ggttefhi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mbfssyhg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3msgbmorp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3pwdwehut.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ixujtttb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3fvbybsgr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3crttxyou.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3syijoxbl.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3rblaergk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dnsiqyhq.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3dlptakss.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qfmchjvn.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3mzmcnjny.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3euoohjwv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zwngmxzg.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3wbyqqewt.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3wwsjeiah.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3pnxqinsj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3yobhtyob.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3rhgnlkfz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ddwvnail.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3phwbnkbj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3jzwzjape.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3lyxvaopd.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3nwymynbx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3swrdowpl.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3fflphiqd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3knpnnaqp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3gpvcpowo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3fbadkjyu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fzefduos.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3pswmjpou.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3pswpkdie.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3jssyiebw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ivryzgbr.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3kthkgjfz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3tyeqzicw.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pgspdwud.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mxrtrarx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3choykhuq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3eomkjvhm.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3yrucnqwz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3jclgssjy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3xbpnjeid.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3eyztdphi.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hfvgfkpc.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ythyxvkm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lndwshpe.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hrfokbwf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rurfkwlc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cdtglhch.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3xaauctza.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3edvbdsos.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3eoajnxbf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kadtqqjv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3xrbhwfcd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ehpwczir.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3tzdeahuw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qroeokfb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3murdgpjg.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3wezozqwt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3topgcmzb.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3tmqnjwko.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3pocgcnda.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3zdjvrzra.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pjaucvvq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3trjgdsta.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3jcxtgjke.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3cqaxdpjb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3bkfdkqpa.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3omyoztbr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ukrgkxja.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ivomtxbk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dxcptwjh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qmdzalwt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3yrczirym.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3othqiwvx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3nyzejkwg.html


<!-- 参考信息 -->