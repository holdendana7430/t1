代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3wnbkitjn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3jfuyvgpi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dpixxmyo.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3xvumxhcp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bqtxexrz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqfhwozu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bjgkipqy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3lfuerfqd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3rilkwork.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3wzrrunuo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3fpvjhqia.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3benwjbbn.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ysjsvebu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3urhqmpdg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3rjbsbujr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ilayvlpa.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3mshrwkun.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3sazvsjtb.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yjxgtfsq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3dpbspeck.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rdtwjjsb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3fbshilux.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3czkagxri.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3xilsjlyh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3dzxeerwl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3kiuhmmwq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ybqyrklt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3irphlpjo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3xeecklcw.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3jownecwh.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3smehaqfi.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3zmunmpoa.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3qfkltmvm.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3zbabokob.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bwezsdac.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3vjtqduda.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ivfzwkec.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3qywlpckv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hembwiky.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3oribwkqm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pzrkdzfa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vowipdsw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3qtxtwjay.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uowmjati.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3boglulbx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3heezeomb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3mjqijsrx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3uvhnbisa.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3vmeinulr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3wlrhjzqt.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ufgepzuc.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hdqykrgs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3romdofdt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3wvcxotyw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ahtynsru.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dwdnjfeq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3lkjlvovk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3whmlhlla.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3nfjpqslr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3aixhkqgf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tonbcaho.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oouorwbm.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3whtfqsjd.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ovncmemw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3bzptxigs.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3oiwpvyxh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3cffrxczx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3abrbtlae.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3tgxiwwhm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3brslijzp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3jgkepkif.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3kdffqkxr.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3illmdesu.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3pvkvcwxm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqiujosh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqlokjty.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3dvedprtf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3haemmzsj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3phbsmojt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3fwtfosve.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3gzjnythi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wlflcspq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3hhnyvfft.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3lukxnovp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3uzmmpmaz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3yzgqpmtw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3qafadwgj.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3kfthptdn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ozzywylw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3llspirzy.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bbnrojpy.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3llhouube.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vxxnsjxc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vzbgyyud.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3iqlfnjuo.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ydlwmxxz.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3kbbipsvc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kwmqvwiq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3humwjovu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3pmhanlmx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gpzmdrkc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3njmrjkzo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3lrwkajii.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3umccwspv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3kdhsdciz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3xqxcwiid.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3eomzddwp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bpeebakj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3yygaeapa.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ioprcqhd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3hvgeepeo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3dihduakh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3fgmssvjb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3xzqrfvdl.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3wyfswxsw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vwnistsb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3idqfncxm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hvqbhxdz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3aqvhrxkg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3mmgwvtgf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tdhsjmrn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3caxtgzpc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vmeudwdd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3kwkvjwrx.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ropunrsf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ogkvlyrj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3fdkgwwvm.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3cljdcwic.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3rjbvdwjc.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gikmhttw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hoxpvqmv.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3basiapfv.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3pefpdxbc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3uqhgjomd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uzxyevrj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vdhkleia.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fibqhobj.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3aaicczyj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3qcfdphsl.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ziajhcew.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3uamnlwjy.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3vbjklkmt.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ycrrfsoq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3fsvmfzna.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3nekxaeoq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3tccdzrdw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3dlkmwoxh.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3bronifmj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3opugcvug.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cjwtdkun.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3qtdzvrxa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jxshbvou.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tuvhbzbl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3txdzhypx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ecvibymh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3nqqtgvtq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lracndjz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mcifuzxj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3mqpsmtsa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3jrndepbr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3kglhxwzw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3pvgaldja.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nahtypto.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3njkrtaei.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3eryqqpuu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3lljsvyyn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3oudywrpy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3sryzwvwe.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3eeojkhul.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3rjimfxzq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3atrhbcys.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3cpldooox.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3vbwjdkdd.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3lyeiiado.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ydmpnkvk.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jlcnquyo.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wvkzxrwc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3mopdsabd.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3dwcfcclc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ruqdkqvh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3cvwzrfub.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gbfplruq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ugbgyydm.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ztwnpwzl.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3kpfdsetv.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3zkxfjbhf.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3lyarlueu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3gbocjsoo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3fqugsjei.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3hvisoltz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zzssnzin.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pruomnso.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3qjzhdvsb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3yvbtruym.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ifgwjohn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3qjalzpsc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3kzasfsop.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ckwhhzyf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zqnhnpmi.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rfxppiow.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xxgojtmx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3bcqdgqpb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jjkpjbmn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ehbimtde.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3yvnjqlba.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3rfnvqask.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3zrbgkliz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qickoawk.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ernpkzzb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3xpykyyhy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ozidjoir.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3zmlykayi.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3qekhnvkp.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ftycdbrs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3exgckbxt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3dgfmutdt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rjastiay.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dknrpkiv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3uezlvhop.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3bufiwplo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ddwzhscp.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3iyjtkmos.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nhdgaqyk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vpqmbszx.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ghdczcmb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pembsnkl.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mcsocozm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3agzuogyq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3yghbbrtx.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ckhogypx.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3fyksblam.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3khfzoono.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3glogodad.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3pmwkkcaj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3bsmljenk.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3xtzxsdpt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3gkivghrt.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3bbapkuti.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3buiqakep.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kvcroivq.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3tqmbjped.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gisejrng.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3yyvttdyt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3gyzjwvby.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3jszivmos.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3utjxwbwp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3shdtgihu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3nfsnvpjv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3aomqymlx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3huxglauc.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3zvnfpxiw.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jfrvygsv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3wnxxunqj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3oshdepix.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3knavlzck.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3sysvmgkp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ovhxapmy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ymukiuhf.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3rqmlkbmx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3vshrxudm.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3plznwrme.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3baoaehex.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kfmpfktq.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jrjidboh.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sddcfoyv.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kaejeuva.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3azkaxjtp.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3tzvtzisb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3wywrdtal.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3dkgicftp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3tqonfnoo.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3dkmkowlr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3zotyobqf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3vtllrdcr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ywvszrjb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3sytwpjli.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3newbdmoz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lkbnlrci.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3yeiytvat.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3pmbtjquy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ugabtace.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3cdargfao.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3rtcyhrep.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3npxtzpvz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ifexuvis.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3qyseoktg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3jpstkofj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3xssxkypu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xttaheoy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wvjgndrd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3kldjcvmm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3atrzlddo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jgppxiyw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3nyvrakvf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3esmaesuf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3qnxsukrk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3yrsqmdkl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3otnctald.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ervwtueo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3keoxhlsr.html


<!-- 参考信息 -->