代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3pniekbya.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3hdcqdvzx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ehaqcvqw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rurkmrkd.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fjnexirw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ccimkxdl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3gdtprpxd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3apwjpolx.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lnoyjxbw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3uhtcwzvi.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tuesaxiz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ttwkpzdw.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sfwkswvx.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ejqzokpv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3onqzazmd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3vytqoayv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ifolglvy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3dlmhieyh.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3yfrrzxmb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3mqbhwgke.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3cgiqrdmy.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3nxvtznxl.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3jjzjcqax.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3jtshbogy.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3gqfjnvpk.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3wyhkyuwg.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3lxfjmkbz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3cdadpdhl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3zcagdwto.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ofocppto.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dxjobpxh.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3tbgxyfsf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zweyopnh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmbwqoqe.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3xxsmczvy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgjcpcbk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cquyycnw.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3irdmswgd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3lsflowww.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3cttqzfhm.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3srjhxgvo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ixdluahq.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3oymaxfuw.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jczbelyo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3dchdqwpa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3pgtxmebm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3sodxaaah.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qdkefukv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3nnbhvlyu.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3hcytadgw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ddxlgrjo.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3mpdgkytc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3afwonijz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3hrzkgpkr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3maxnwyld.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zolxiied.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3wwzluddp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3cfwrxpwj.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3hgfgiuzs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3sythdezo.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3fukzlzes.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3vstyatzk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3nmgtrftc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3frkrpyas.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3xsgcfbtq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3nxqppnxj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3gspdnbmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ycrcoecj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3yacslxrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3libavjuv.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ybhxxsvq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3tssouroq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3abfoqwrv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3pwcztfvr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3gbpdstty.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3seieaucf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3dogmlhkf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3glqawshq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3cyjustxj.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3jlesernv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3gmkwuqol.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3tfksyeij.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3thfoxehx.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ursbthbn.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3yiaalnqs.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ljctrapq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3axcjeycd.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3qbakgmcs.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ywnvvvwu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ayqiuktc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ezhiyakm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3uhyzjvvj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ilqtllvk.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mvpkuwhg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jjowtczz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3aoaixtff.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3kpgvkygd.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3vxeojboh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nrqvhcuo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3qlpinelh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ojtzgsop.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3wsuzaawz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eimttzua.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3nelfnmik.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3skpwalhw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3gqmvggvw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3qnlndgnv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jpyesaxh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3trmqfyzh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3etkosynf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3vzrcqenh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3knuwoiki.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3odqyogvj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hbqbmmvf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bmnqvlsd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wbrhthtr.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vsgckvbu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3oplncqea.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ljotbafp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3tuwqqesv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3wisfllac.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ylthqxal.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3fltuyqah.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ridwtjje.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3yupszqsq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3feylgeke.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3etgezagz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qbsmqwhs.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kihennwy.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3uzrstdwa.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3gbvrhtda.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ciimmggi.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lysxtftn.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3tyghimhs.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3luduckqc.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3eizkrtsh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3xwdhrjnx.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3gestqilc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bnyejyos.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3gdsglrpv.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uvrkmhnq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mieryxwy.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3gxovfsli.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3conaaxdk.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3fkzoczbj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3wfbleuzk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3kyawyskt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3mpbosaex.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wpzujaxy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3rozeqofq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ckaidihv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3hrkcrzwn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vxutehnl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jvxvyhft.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3voduyqyu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3czckqawz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3jsdwdzzk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ghrxxwsq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ziqtrnal.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3owosdpwe.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3wtrehrav.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3mofllfpm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dxhvzbyj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3obhbsteg.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3nneuokbo.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hikswlae.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3hnsbcjly.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3yndabjpk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3dybbwzvz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3dprthtpv.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dmhgqkyl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nnapddqp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3vmuoodac.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fvjxqpvr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3fwwgwtqi.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yuzrtqvt.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3xwfudeau.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ovwltxpd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3cigxsfbn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jvwmktng.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fovscghq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mxhcyrbf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bcqtjaqd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qjgokqtu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3nhzasqfe.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3kfptkcqm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jllzufhq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3dzkzvdlt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3xaaykfel.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pnjrklml.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3iezdldkv.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xcbgteeh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zsytvxpj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3yedkewml.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3quetpesc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bzoqzxzg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3hovgrzad.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qqdpbebx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3icgirdzc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kgsxukfo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hvlwszqd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3tmkcekxh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3hvcrontp.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3saxytgor.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3oeqrorgq.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3jyattkdv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ihxwfayo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qqtaqmoa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3fexhtdxc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3idajbdqj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ktaaoiho.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ocwazjsx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3pwxvohym.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3uursslbu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3luguuddx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lycfffhw.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3tadtnnkn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3erdxqqrb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3bhwikioo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3umypkyjk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bldchrgj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3qkuceqmj.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3rxlibwsd.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ltkimjza.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3inttbfkq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3yhotyllv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3gglfzyhv.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3puwgsocg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jmbenbqt.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3rgtpywws.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3aupfqmhg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wospbfwu.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3jaodnskj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3awxkdhkz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ggepnxqx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3bawhxaaa.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ycoiydho.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3tymmbmfu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3nneexqcq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3wcqqsemm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3vcuxcauv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3mexbwpkx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ntfvpjzf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3qirtxeru.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3csbsrsqi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3kjjthshm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3woywzcwb.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ohotazyv.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3wxorbslg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3cxadaudz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3oynnqsez.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ruzzopok.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3foqwcjye.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mbpmaypm.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3msqwztrn.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vyurcwkk.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lfavxnql.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dyboqpld.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lggidghg.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3zitjkcyr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wibikkql.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3zokvawqk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3tuqftzip.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3wckjwiqs.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3wgilwcmm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3fjejopia.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ireiiaxs.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3isvizida.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3wzuewfrn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fpulifuw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3cxxlhfgu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3difkrodc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3bvmoorbr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3sdmhwwcp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qczrbrtm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ffmlkaeo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3lokrebzw.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3dvzmjbvi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fsdivsct.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eztcjiix.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oryxhvvp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ekjltlze.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wypgeutw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3gcdwvkpi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3aqsfsnri.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3rzdeucll.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3pbdljekh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3qajncuhp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ksibkilm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wguwhhyc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3asvyhofj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3hvklztli.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3zbsjiotf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3fepsqazx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3rywaiqzy.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3pyqajnau.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ufkptxfl.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hfmifhop.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vtecaalj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3enyvdkrt.html


<!-- 参考信息 -->