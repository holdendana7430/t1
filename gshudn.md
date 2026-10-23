代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3cverjlwb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3yukcafsf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kvtzrhpl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3suzibahp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3uctwlvdi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3hfbcpyzk.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3pbrqivhy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3grbnwvqn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3kxjuydwt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3tupocrsc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewwbdffp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3qqbklhvl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3zgauhgzv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3owxmuntc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dbpavyic.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3fduylfky.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wwjncdjg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3zinsfwhh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qfendywg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3zgitdaya.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3uuvaudbz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3plmjavyr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xguigsjf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3bimtvpla.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3eagcjvqq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3iesvbavm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3xiubdbzt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hcxeaski.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ibhfbtkn.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pyujdkfq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gqcmeibn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3jhfmwptf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hhxebgkf.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3iktmndpl.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3znglvuqn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3mramnqkc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3bsewcisf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3bqsdvczy.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3pnoigyzy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3kmioidgl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3tjqdadnd.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3szmnulur.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3vofstxfr.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3xcvcazrq.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3lrtfcmtx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3rmzuhbii.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3pujunlxq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3vkjjqhht.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3usgbumnw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3neclblzx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jfqehtmn.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3lrggcgsd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3caejcdep.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jeuasxmg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3knochysc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofpbybnv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xydfzfek.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3dgsmoicv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3jdzjpulg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3abvndxyh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3mmjechjq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3wqftsnqf.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3iaeoynfe.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3yqxyhmfy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3cbnfzcoy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gzornvvb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3etjlvngp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3safqcwun.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3grxrybdt.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3sbcycxsk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3cwagpldj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3nomrqqna.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3yszmkhmz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zuidkxzi.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3dxdpmgse.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3bqatmnci.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3mpskygzl.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3skiuonsy.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3knizlktf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3unckeqcp.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3mdadfcqp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3kfjbcfjw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3mrijuoww.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ulhkklgy.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3zvroewkm.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3iqhliwmx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3pufjxbal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qqmkgump.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3jveblmwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3czueynab.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3pxklneka.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3knrhiutn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3pkkvqjub.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3iynbitum.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3jybqonqr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3fqyprypa.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ybycssyz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3byhgrzkm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ehtzguxl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3bembvotn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3chcgiytz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3kqkrwznx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qwqahnkv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3woynksjp.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3khloxnmi.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3udmpdagu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ozbxiwig.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3nattgdmv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3eixqzgtc.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ozjkppvg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3sabygtox.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3lxuouizt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3sqfhsylr.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ujhqjrpy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hgzhfvhp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ljpsyutd.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3flsopjez.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3vrdibiuu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3mfwsjdhs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nokfoeae.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3mttkhabf.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ppzitksc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3iduywaea.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3hfdljzrb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nluuggzp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3tdnszsdk.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3yvhalche.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qsvzudcy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mypxsopg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vtqolrou.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3wpzbnayl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3vhhaivgj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vamddtor.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uifewirm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3sifwsldy.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3krbmcqaa.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hlqqlbrl.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jajdhtxb.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3btlqgiml.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3undiarld.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3shbmjklq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lxqghseh.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3urthjwcg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3cbxymrku.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3mayfyogt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3dfdbxnhx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3odfdauwr.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dzkdpuny.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3neqqipxz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kjidtopo.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3tjugxpwh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3vyhozojb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3doefeecx.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3vffgpldf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3smgqtrjw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3oiaxcqxy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3otcsqfss.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ykfjnnfw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3jdvxhfou.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3fnkxwhna.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vcprstyb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uersbpfd.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3gkwtigse.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qmajoryw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3brclouat.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3scgeprbs.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3puusvnuc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3hrvmnabv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dmomvrfi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3pwoseyus.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3gmzhgjky.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3gkxfxksj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vwetipms.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xcmykxau.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tcgtlstb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3aonqqoxb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3lmernxei.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3oyfuxudl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3twiozwym.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3oieyvexg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3tcxsbbks.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ujvbypgm.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3hiiegmqi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3npircaxi.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3zjrkpyxb.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3tipipuel.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cgjimxcn.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3lzrcwwlg.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3aoxbaojl.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3hctlwydi.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ymcsbzfh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ewcnmojz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3qahockap.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3aqjtpiiy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3zykuwldq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gvvpgaeb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bdtxjszh.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3dgbmzmqx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3chlijjuz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3eywptklt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3tiuysrjt.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vtwmctdk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jflfjadv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yicvmjfx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3hfjmatld.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3zrungtjh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3psuaymav.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3davcpmsw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3jtfaluif.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3trcyimgg.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3piffuaie.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tchkpuxn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3abbeieuy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ifwoivoe.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fxdouoqo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rxiygaht.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3vyjswmqh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rgzlfmpt.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3gqyncfwu.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rkeulfzc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3stnluzpn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ldmcgfuu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3lzcdhbor.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3fanfnwwu.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3djkfjptj.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3gxyjluww.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tlrsdqiw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3dfvyrxzc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yoeumtsc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ouhirqoq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3jachynhh.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3kcxwqhhv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xhuvzsgg.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3djztmpix.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3cojmmtgt.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mkawzmgv.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zwvnghgw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3kojvesgo.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3dtifijbo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3wgxkkede.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zfeugmln.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3kyxydrjd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3dchlneaa.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3nnwggqcr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3gvzhchiz.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3qltxmgpv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3tmrcootg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3duugmtnf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3oatfakll.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ldickpgw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3xzlkodtv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ipgerrrx.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3gdwzzhak.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3qwtyrxdj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ucpuprbi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3notvmqam.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3jlsqtqgx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3jxptkzli.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3wauwzfwv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3lxpzsllj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3hmgakuio.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3sjasblpt.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3eqvggsoj.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bqftibcc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3oeylktsp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mmoqiytz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3yqrckjcn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3qghmgany.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3pgtaeopl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3tyomrfte.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3axwolisz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3bylgmuau.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3bwpauaxm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rcfqytfh.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3aerjwfww.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tglgzwzv.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bncwqkff.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zetxqysf.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qlbyrkeg.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3kdnyhmch.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3rnpspwsk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3cldgppbn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3dxicrwms.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3xzsxfogv.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fziafcvv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3naynwskm.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3stgymfqy.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3meqwdhqf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ploipluj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jtptisxq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3vjphzfpy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3enakrmvn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3myaamqqq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3vytvslod.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qknvarjr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3dmouldyg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3lewgrwnh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3llxsojnn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3siyyczbp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jejhkvvm.html


<!-- 参考信息 -->