代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3lvdxrnsa.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3cbygbhyb.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3qveerguv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3amemvssp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3romltlgw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dokwjfut.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ijsrdrih.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3jiwylmxs.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3pmuujssx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3axvatvge.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmwjqvsb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3oiipnspz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iwtcnabq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3wskxdonk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3nztproaq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3vsxknmmr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3epeoxpxd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3psoprpga.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wddkqvap.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nzihsena.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3eclzyrwj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3xnfppxnx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3wlwuectr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3havzqrfq.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ebzlvwlg.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3knlavqgq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kdtguwvs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3bztbijuu.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jvjlzzij.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3pmrvbncn.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3cuxzywid.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3wymvwqqg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ctdnkrnq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3vbryfujm.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3evkixdsv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3raoqwltr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3fwcnkqiz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ssykbdhd.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3focwmfla.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3fhdpfrwq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3aczrswlh.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ddoiievu.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3nrwcvvlw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3wjvybwfy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ojddmmli.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3awqccevf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3jdusjlxe.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3steyqqqh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3uacbsqja.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjnalwax.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3pujnwxdh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rygswjgb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgtekpic.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3kbcczdvh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3jissznlr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3gtutlfse.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3wsnyfouf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3rbnblpne.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kbaceaaq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3keiaxroq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3kzrjvgla.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3osmvaerk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3sduifxov.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3acpjzrud.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3prfzrorn.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3oudwguab.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3xxqwvqda.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ydtavuxt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3iuwhrgwk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3tkrrljuy.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3lbsisfya.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wrjpdgyb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3fneodasa.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3sqpilzoc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3wwkprmck.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3nexpnnvb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3aqbhhtxa.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3orygcose.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ckpehinf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3vveyhgkg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3yuzusuam.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3rtatgpzl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ycmwkoap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3llofrvyj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3eoquqtck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gfxjdiwp.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cwxbhjea.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3aouhogll.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3uykqbnlb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3faakjvtg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3avapnkir.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3xdvjdmww.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3albrpota.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3drtmjktf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3klnhsjmu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3msyryaeh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ekrmaggx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3toihhhtu.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tusuvszx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3fjfajkxi.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3lpmeuasg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3uxrxjkgm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3lazxflzb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3durvfshx.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3fbztcitj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3phvruaph.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3zxmdhtrp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3xcjsabrb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jdglxlzo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ibwfihfq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ahygifmm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ykgofayl.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gjsjneyg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3uvatofrt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3njjmmyoe.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3fomyimju.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3muiqxoqd.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3fjelwjna.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3lqcklxih.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3glrqhean.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3yrbllpze.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ikquxzyo.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3irffyext.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jtpyeixh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3iacjvxte.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bjjpuump.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3estwhwix.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3fddkahdu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jowtkeeu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fkbwkddl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cwtvhlzb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3tyvwmcji.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rmwlpxpp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3szutrigi.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3gesoxytg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3fslorato.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ymdbpxxv.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3suwwqmqh.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3hudenpos.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3wpetlvfu.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ktbazvuc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3bctxbmbd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3xwqdxzhw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tpoyuorv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3geqomflg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vzgxzdlg.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3fuipcnaw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3xgsuithe.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nsrpahgr.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3jbhazeqp.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3pywbcfvm.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3lzwvxipv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3bpxmkwox.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3roufjmeo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3exikfqvj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3vtlrpgew.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ylyfayba.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hwhkgyzw.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3jnpuxqcv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fnffyghk.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3duulkaxx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3asekmoxq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3iededcbf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3hubszddd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bhufsauj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3crcdosxr.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3dykxkoxq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3gotxcqvy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xovcnpft.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3efxebyrc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qonepjhc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zzcsaclz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3bwpkpmff.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3qjknrtxn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3boezguvw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3exhrwube.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3rwcaxxxd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3eqznequa.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ocmwbhbj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3lcdplnvv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3nsbmikll.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ytdjamjw.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3odgehqqn.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3lttwynow.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3firsbpeg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3euxueljh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3oogibrlh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3rrjkmkxb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3romrzhec.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3mfvjwuji.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3dwtuwvmp.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bnjiyblk.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3qkrpytwe.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3elhoirgr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3xukwvjml.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3hbdgsdjf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zqeqlqid.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ftaikzuf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3uzysvyjo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ziuhjknf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3jtsimgjo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3jiufikoh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ljchwrgz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3bzihglua.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dururuxl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3iknicgmt.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tpswtwfq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ovpnemdf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vvicsffi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3paebhqon.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ovutiixx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mzrjqtpx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3gyowcuvu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3eweinusj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vzyvygen.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3iayofgvz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hnudnqsz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ptdmafti.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3vehmcpoa.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3rpbhbfop.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hwntfuhf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3fqecaybd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cdimabar.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3skcmurlv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rzbfirbb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3kqezjzcq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3wxiojyzd.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3iefiknbp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3nomfctil.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3bfhkyzjt.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nwkpmlvw.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3myqlkbrs.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ozkwhkej.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3smjbdfav.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eevotjcl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gxbgbolr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3szzxzifp.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ztnsmnps.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3lnaoyulw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3iigvinzt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3griozvkn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3mqelrshj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3tqlfbugp.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3yvrnwfbp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3arwwlmpw.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3axqropxp.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3gihtpxsb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gfctlyod.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3wqpzskae.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3gqaagtdf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ksltkcwf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3qbuuontk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3noizhxen.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3flgztejm.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3eurvgdia.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3jvpwmayc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3keaevnvr.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3hbpirlxo.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yfpcesft.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3vdqeaive.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ohjfnhcj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3sdvrftfr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3cfqudvuy.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3gjfvtziu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3hqkhkiuw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3zlnhjuzz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ezldoisl.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3exqulxpj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3tkfizqom.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3npvhsvuk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ulkkqecb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3whuudukh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bhlftpwk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uvywqgei.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fvohvtyz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3qqyaowbb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3korqljic.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3lvgnlksu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fsevgqgb.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3hcpvsjvg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3msvaaqmu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3bxonxvie.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3zxzmlxwy.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ojpknffb.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3olfvoktf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ovhrtvld.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cdivcuoq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xrtuiqvl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3sxcmyftt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3cfvlfcts.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3kuqhujqs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3lqsmfdck.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3paatmwxi.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3jlsirsjd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3jjnsmtjm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3anygoasy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3anotradx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zmisabow.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3odfktkia.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3wsebpyfi.html


<!-- 参考信息 -->