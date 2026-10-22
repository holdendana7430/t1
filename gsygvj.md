代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxpzomzz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2kdknomnf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2shabyuzl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2xeoamfrg.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qpcgprsw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2lxvpviry.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2awjgwwmj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tlwfxlrp.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2gxjqbolc.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cmweydak.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xrvnvwcx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2dthbsbbf.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rnpitkmv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2fkwmuuui.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2xvevnjkq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2sxuvocbh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2dyodmkkn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2smcenzwy.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2afigmxkl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ehembvnd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2izyczfzj.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2hnduoxkx.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2vfozjntv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2yzbiisfc.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2woboqisr.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2xcgtrcgx.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2kuzebwcv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2rzocflim.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2lgubyjvq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2tocsozij.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2rwqsilof.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2invcdnjd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2rokwnnna.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vjggluxz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2qlrihdmf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2juxogdzo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzvgperc.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2omrbfdur.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2epqtuhtb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2szplznto.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2caaqeswq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2oeseyexv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dhglhtrc.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rbhpwtjw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2juctasci.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jzzdztpu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2dejyzccl.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ytmggbvd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2vecvpsfd.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2gxjfovhl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2yuvoqzby.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2fjonccfy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cubzikhr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajlkhwfl.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2xhcktyye.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2xvhslvfv.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2uttfhmfz.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2xzszcfif.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2cdfgxgxi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zgkwjrgn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2itglpfdm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2opdpfaia.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2sqzmnjbw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhesijpf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2swdomjqb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ykcwjids.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rpvtdglr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2utynutzt.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2eqhtxdfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rgidiszc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2aieuftko.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2yqrhbvxb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ntooiqld.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jbmtytis.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2yusqjewb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2uwbgwzdg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2djkbdzel.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2iyvdmecc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2yxhrwnsf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ushddzdw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ousocyut.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jpncgvmo.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rluzughk.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2whjeexuy.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2hdipzigo.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2cceeezyo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2knfzixnk.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jnbqbvnr.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2qfjbltft.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2azkhdsfv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2yjtynclt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2mkydcurw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2stzhtizs.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nyummefm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2znjyijzb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2gwtxmgve.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lwlodwcn.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2bpowqske.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xizqrhgy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2wsbtusoh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2flsbynfx.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2uqfzqwwj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nrnxpmxy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2fjnjllrk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ejbnbkyl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2rxrweooj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2bruimibi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jwcphomx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2oqaafevq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rkljipgg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2advkkbun.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2cumpiqaf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2abhpxifd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jnadlxus.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ipsilqee.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fxyjxirp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pqfcgjvl.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wifewbcc.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2knqoasow.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ymnkpfrs.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ewiilqsi.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2knafbyeg.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ogmxfgou.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2jmhiehbd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2faxhzpdf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2fvgnizpv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cszxager.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bwmegizr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ssjunigg.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2utdlsfoc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2zhzzneag.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2hsqjaytb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zuaebogf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2gqphqtzt.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2wlokffxv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2wwhojgdq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ybjpgiva.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2hxwocsco.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2dauwfode.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2luaixxgu.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2moetvers.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mhwxozcz.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2rutewbob.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2qmummcqg.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wctygrcn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ewqewnab.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ggunulyw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2jmaycssj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vgfglfvj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ubwqfqna.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2bxojmxwj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2atkgsnfa.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ubcbnsot.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jfbtkjsd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kopfsqgu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2juxfcdcu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2kcnljhmw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2yghvorzd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2qmzrlavs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2qxgjaytp.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2jnpvphfx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2lsaekjxe.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2pjedhewg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2osaftpnp.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2wtkrkinv.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tecfoxgh.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tuhigouc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2abvptsrx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2bmhxakqr.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2pjvcgnhc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2nrlujbfc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rthdtnuk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ubzjczoa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wiybqvci.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2bcybjozy.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wjhotvbl.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2mvqvkpbu.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2nenzqjie.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2hhwgyadv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2moqhjalt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ipgygkut.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bdbulmma.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2rxczhcdh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sapeegnp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2cpeacuns.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2rlqbbrlj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qkfgifta.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2yjtriweu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2czragkiq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2lvqyxwlj.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aienhjpx.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hvbucuag.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2lpyqglck.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2cjjqszdh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pglufkzz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ooqcviaq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2airvkuus.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zergoucr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vmmtoqnc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bnkaeqrn.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qkuadhrj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2euoyxzqk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2sjtultwp.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2gqewfvmq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2rezptnui.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2xcimmhfh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2afsycrsc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qfbakqpb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wmitackr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2cykhmdfh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2tgnxhsqn.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2yhmkfbha.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2jghlvedt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2kgvnrlat.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xqmtcaln.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oawadseu.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2prghaaej.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2golzwjlt.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2dzxrrwoh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2jdtzaomy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qhmcttbh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2fdmnyatk.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2zdwaxbng.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2eocotijh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2qseyqqqn.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2hylzntiz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2hnawoioz.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2lgistvpb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iehlqfum.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hipclqpd.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2bdzkwwgi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zzifucbo.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2bbnwvreo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ckdvthdm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2mgdzahzj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2akdrlcjb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2smhaobxq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2nsznarzz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2vzrptipg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ylchyzhl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2jqtafreg.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2qpnclrrz.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dasbgqhl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nmkgzulh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qjogyvry.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xciggusj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2emeaeecv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2xhtgvxak.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2tfqedhcf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2sqkrjtvj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2qidwcfwd.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2efcuwcdv.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fihfykxi.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xezrhrkp.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2atiiuovl.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gfpagnps.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kecglkcp.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2lkcixgrc.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xrkcuobx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ofhxwlic.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mdvmpajx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2dfbuxybd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2nfklhqht.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2kufkisso.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rbclephs.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2sldwbclg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2wgzgohhc.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2gfhpraaf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2kuwlaezl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2elswfbmf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2emlswafh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2kugoxbaa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2uhvgffam.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2qeoasunk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2svhkchfq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2mhnyhrvr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2dsumyumo.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2izjjabop.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2syfpguqs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2iummxgyi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2dwybmpup.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zxaqrqvh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pbuubprs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2abaxonvu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nqenghiy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2itnwtony.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2vvibnqqd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2hpzxjzsd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2uojeopaz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2auklspkb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ynuoaeod.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bykoueoj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2iigjrnbv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ifbyymda.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uhyfudgk.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2xajdyoym.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2jqanuieh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2soczccpq.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2sygalxdw.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2robcplpq.html


<!-- 参考信息 -->